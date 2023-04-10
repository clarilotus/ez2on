---
hide:
- navigation
- toc
---
<link rel="stylesheet" href="https://unpkg.com/element-ui/lib/theme-chalk/index.css">
<script type="text/javascript" charset="utf8" src="//code.jquery.com/jquery-3.6.4.min.js"></script>
<script src="https://unpkg.com/vue@2/dist/vue.js"></script>
<script src="https://unpkg.com/element-ui/lib/index.js"></script>

<div id="app">
    <template>
        <el-tabs v-model="activeName" type="card" @tab-click="handleClick">
            <!-- 4K BASIC -->
            <el-tab-pane label="4K BASIC" name="4b">
                <span>
                    <el-input v-model="searchTitle" placeholder="搜索歌名" style="width:240px"></el-input>
                </span>
                <span>
                    <el-input v-model="searchArtist" placeholder="搜索艺术家" style="width:240px"></el-input>
                </span>
                <br /><br />
                <el-table ref="filterTable"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="850" style="width: 100%">
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录" :resizable=false width="64"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }]"
                        :filter-method="filterHandler">
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="75" sortable>
                    </el-table-column>
                    <el-table-column prop="bpmrng" label="BPM 变动范围" :resizable=false width="115">
                    </el-table-column>
                    <el-table-column prop="B4EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B4EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B4NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B4NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B4HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B4HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B4SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B4SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 5K BASIC -->
            <el-tab-pane label="5K BASIC" name="5b">
                <span>
                    <el-input v-model="searchTitle" placeholder="搜索歌名" style="width:240px"></el-input>
                </span>
                <span>
                    <el-input v-model="searchArtist" placeholder="搜索艺术家" style="width:240px"></el-input>
                </span>
                <br /><br />
                <el-table ref="filterTable"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="850" style="width: 100%">
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录" :resizable=false width="64"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }]"
                        :filter-method="filterHandler">
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="75" sortable>
                    </el-table-column>
                    <el-table-column prop="bpmrng" label="BPM 变动范围" :resizable=false width="115">
                    </el-table-column>
                    <el-table-column prop="B5EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B5EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B5NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B5NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B5HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B5HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B5SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B5SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>

        </el-tabs>
    </template>
</div>






<script>
    var url = "../test.json";
    var request = new XMLHttpRequest();
    new Vue({
        el: '#app',
        data: function () {
            return {
                "tableData": [],
                "searchTitle": '',
                "searchArtist": '',
                "activeName": '4b'
            }
        },
        mounted() {
            var self = this
            $.getJSON('./songlist.json', function (data) {
                self.tableData = data.songs;
            });
        },
        methods: {
            filterHandler(value, row, column) {
                const property = column['property'];
                return row[property] === value;
            },
            handleClick(tab, event) {
                console.log(tab, event);
            }
        }
    })
</script>