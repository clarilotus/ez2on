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

.ez-1ST {
    text-align: center !important;
    color:white !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #724E00, #0A4900, #002484);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-SE {
    text-align: center !important;
    color:white !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #000338, #002BA9, #000338);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-2ND {
    text-align: center !important;
    color:rgb(255, 232, 99) !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #390007, #980020, #390007);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-3RD {
    text-align: center !important;
    color:#7DFF2E !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #191919, #383838, #191919);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-4TH {
    text-align: center !important;
    color:#FFD969 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #0132A1, #001727, #0132A1);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-PT {
    text-align: center !important;
    color:#FFD969 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #6D6CA1, #312C40, #6D6CA1);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-6TH {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #FF2B2B, #34364F);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-7TH {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #FFA32B, #FF6700);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-2008 {
    text-align: center !important;
    color:#FFC924 !important;
    border-radius:0.4em;
    background-color: #08284D;
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-2013 {
    text-align: center !important;
    color:#90FF00 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #003A49, #08284D, #003A49);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-2021 {
    text-align: center !important;
    color:#40EEFE !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #03212D, #006C83, #03212D);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-TT {
    text-align: center !important;
    /* font-style: italic; */
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #00120B, #004E35, #00120B);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-CV {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to bottom, #D655DF, #9D26C5);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-PP {
    text-align: center !important;
    color:#f3efff !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #1A0032, #5701A1, #1A0032);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-O2 {
    text-align: center !important;
    color:#000000 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to bottom, #14FEDB, #9CFE6B, #FDFD1A,#FED815,#FEBB11,#E58220,#B25563,#893F9D);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-GC {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-color: #F9618C;
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-EC {
    text-align: center !important;
    color:#014649 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to right, #808080, #EAEAEA, #808080);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-FT {
    text-align: center !important;
    color:#000000 !important;
    border-radius:0.4em;
    background-image:linear-gradient(to bottom, #FF6E43, #F9AF17);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-NW {
    text-align: center !important;
    color:#000000 !important;
    border-radius:0.4em;
    background-color: #FEE600;
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-TC {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to bottom, #000000, #760000, #F50000);
    font-size:1em !important;
    font-weight: 800 !important;
}

.ez-EV {
    text-align: center !important;
    color:#FFFFFF !important;
    border-radius:0.4em;
    background-image:linear-gradient(to bottom, #21525A, #272727, #800F2E);
    font-size:1em !important;
    font-weight: 800 !important;
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
                    :border=true :fit=true style="width: 100%" :lazy="false">
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
                    :border=true :fit=true style="width: 100%" :lazy="false" >
                    <el-table-column prop="id" label="#" sortable :resizable=false width="54">
                    </el-table-column>
                    <el-table-column prop="dir" label="目录 " :resizable=false width="70"
                        :filters="[{ text: '1ST', value: '1ST' }, { text: 'S/E', value: 'S/E' }, { text: '2ND', value: '2ND' }, { text: '3RD', value: '3RD' }, { text: '4TH', value: '4TH' }, { text: 'PT', value: 'PT' }, { text: '6TH', value: '6TH' }, { text: '7TH', value: '7TH' }, { text: '2008', value: 2008 }, { text: '2013', value: 2013 }, { text: '2021', value: 2021 }, { text: 'TT', value: 'TT' }, { text: 'CV', value: 'CV' }, { text: 'PP', value: 'PP' }, { text: 'O2', value: 'O2' }, { text: 'GC', value: 'GC' }, { text: 'EC', value: 'EC' }, { text: 'FT', value: 'FT' }, { text: 'DM', value: 'NW' }, { text: 'TC', value: 'TC' }, { text: 'EV', value: 'EV' }]"
                        :filter-method="filterHandler"><template slot-scope="scope">
                            <!-- <el-image :src="'./diricons/' + scope.row.dir + '.png'"
                            style="vertical-align: middle" :lazy="false" /> -->
                            <div :class="getClass(scope.row.dir)">{{ getStatusText(scope.row.dir) }}</div>
                        </template>  
                    </el-table-column>
                    <el-table-column prop="title" label="名称" min-width="300pt" :resizable=false sortable>
                        <template slot-scope="scope">
                            <div style="display:inline-block;vertical-align: middle">
                                <el-image :src="'./minidisc/' + scope.row.name + '.webp'"
                                    style="width: 38px; height: 38px;vertical-align: middle" :lazy="true" />
                            </div>
                            <div style="display:inline-block;vertical-align: middle">
                                <div style="font-size:12pt; font-weight:600pt;vertical-align: bottom">{{
                                    scope.row.title}}</div>
                                <div style="font-size:8pt;vertical-align: bottom">{{ scope.row.artist}}</div>
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
            },
            getClass(dir){
                if (dir == 'S/E') {
                    return 'ez-SE';
                }
                else {
                    return 'ez-' + dir;
                }                   
            },
            getStatusText(dir){
                if (dir == 'NW') {
                    return 'DM';
                }
                else {
                    return dir;
                }
            }
        }
    })
</script>
