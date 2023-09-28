---
hide:
- navigation
- toc
---

# 歌曲列表

<link rel="stylesheet" href="../stylesheets/element-ui.css">
<script type="text/javascript" charset="utf8" src="../javascripts/jquery.js"></script>
<script type="text/javascript" charset="utf8" src="../javascripts/vue2.js"></script>
<script type="text/javascript" charset="utf8" src="../javascripts/element-ui.js"></script>
<style>
#_1{
	font-size: 0.001em;
    line-height: 0;
	color:transparent;
}
.md-content__inner {
    margin: -38px 0.8rem 1.2rem;
    padding-top: 0rem;
}
</style>

<div id="app">
    <template>
        <el-tabs v-model="activeName"  @tab-click="handleClick">
            <!-- 4K BASIC -->
            <el-tab-pane label="4K BASIC" name="4b" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='4b'"  v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="530" style="width: 100%" :lazy="false">
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
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
                    <el-table-column prop="B4SHD" label="SHD" :resizable=false width="75" sortable >
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B4SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 5K BASIC -->
            <el-tab-pane label="5K BASIC" name="5b" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='5b'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
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
            <!-- 6K BASIC -->
            <el-tab-pane label="6K BASIC" name="6b" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='6b'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="B6EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B6EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B6NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B6NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B6HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B6HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B6SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B6SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 8K BASIC -->
            <el-tab-pane label="8K BASIC" name="8b" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='8b'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="B8EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B8EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B8NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B8NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B8HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B8HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="B8SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.B8SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 4K STANDARD -->
            <el-tab-pane label="4K STANDARD" name="4s" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='4s'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="S4EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S4EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S4NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S4NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S4HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S4HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S4SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S4SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 5K STANDARD -->
            <el-tab-pane label="5K STANDARD" name="5s" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable"  v-if="activeName =='5s'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="S5EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S5EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S5NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S5NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S5HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S5HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S5SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S5SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 6K STANDARD -->
            <el-tab-pane label="6K STANDARD" name="6s" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='6s'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="S6EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S6EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S6NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S6NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S6HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S6HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S6SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S6SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
            <!-- 8K STANDARD -->
            <el-tab-pane label="8K STANDARD" name="8s" :lazy="false">
                <span>
                    <el-input v-model="searchTitle" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索歌名"/>
                </span>
                <span>
                    <el-input v-model="searchArtist" style="width:320px" clearable prefix-icon="el-icon-search" size="medium" placeholder="搜索艺术家"/>
                </span>
                <br /><span style="height: 10px;display: block;"></span>
                <el-table ref="filterTable" v-if="activeName =='8s'" v-loading="loading"
                    :data="tableData.filter(data =>(!searchTitle&&!searchArtist)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&!searchArtist)||(data.artist.toLowerCase().includes(searchArtist.toLowerCase())&&!searchTitle)||(data.title.toLowerCase().includes(searchTitle.toLowerCase())&&data.artist.toLowerCase().includes(searchArtist.toLowerCase())))"
                    :border=true height="550" style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'SE' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" />
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.png'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="false" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:5pt;vertical-align: bottom">{{ scope.row.artist}}</div>
                            </div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="bpm" label="BPM" :resizable=false width="140" sortable>
                        <template slot-scope="scope">{{scope.row.bpm}} {{scope.row.bpmrng}}</template>
                    </el-table-column>
                    <el-table-column prop="S8EZ" label="EZ" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S8EZ}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S8NM" label="NM" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S8NM}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S8HD" label="HD" :resizable=false width="70" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S8HD}}</div>
                        </template>
                    </el-table-column>
                    <el-table-column prop="S8SHD" label="SHD" :resizable=false width="75" sortable>
                        <template slot-scope="scope">
                            <div style="font-size:14pt;font-weight:700pt;text-align:center">{{scope.row.S8SHD}}</div>
                        </template>
                    </el-table-column>
                </el-table>
            </el-tab-pane>
        </el-tabs>
    </template>
</div>





<script>
    var url = "songlist/songlist.json";
    var request = new XMLHttpRequest();
    new Vue({
        el: '#app',
        data: function () {
            return {
                "tableData": [],
                "searchTitle": '',
                "searchArtist": '',
                "activeName": '4b',
                "vheight": 100,
                loading: true
            }
        },
        mounted() {
            var self = this
            $.getJSON('./songlist.json', function (data) {
                self.tableData = data.songs;
                self.loading = false
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
