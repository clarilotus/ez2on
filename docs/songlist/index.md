---
hide:
  - navigation
  - toc
---
# 歌曲列表

<link rel="stylesheet" type="text/css" href="../stylesheets/jquery.dataTables.min.css">
<script type="text/javascript" charset="utf8" src="//code.jquery.com/jquery-3.6.4.min.js"></script>
<script type="text/javascript" charset="utf8" src="../javascripts/jquery.csv.min.js"></script>
<script type="text/javascript" charset="utf8" src="//cdn.datatables.net/1.13.4/js/jquery.dataTables.min.js"></script>

=== "4K BASIC"

    <table id="4blist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th style="width:28px" >序号</th>
                    <th style="width:28px"  >目录</th>
                    <th style="width:28px"  >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th style="width:25px"  >BPM</th>
                    <th style="width:40px"  > </th>
                    <th style="width:22px" >EZ</th>
                    <th style="width:22px" >NM</th>
                    <th style="width:22px" >HD</th>
                    <th style="width:26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#4blist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
                ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '4BEZ' },
                    { data: '4BNM' },
                    { data: '4BHD' },
                    { data: '4BSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "5K BASIC"

    <table id="5blist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th style="width:28px" >序号</th>
                    <th style="width:28px"  >目录</th>
                    <th style="width:28px"  >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th style="width:25px"  >BPM</th>
                    <th style="width:40px"  > </th>
                    <th style="width:22px" >EZ</th>
                    <th style="width:22px" >NM</th>
                    <th style="width:22px" >HD</th>
                    <th style="width:26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#5blist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
                ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '5BEZ' },
                    { data: '5BNM' },
                    { data: '5BHD' },
                    { data: '5BSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "6K BASIC"

    <table id="6blist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th style="width:28px" >序号</th>
                    <th style="width:28px"  >目录</th>
                    <th style="width:28px"  >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th style="width:25px"  >BPM</th>
                    <th style="width:40px"  > </th>
                    <th style="width:22px" >EZ</th>
                    <th style="width:22px" >NM</th>
                    <th style="width:22px" >HD</th>
                    <th style="width:26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#6blist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
                ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '6BEZ' },
                    { data: '6BNM' },
                    { data: '6BHD' },
                    { data: '6BSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "4K STANDARD"

    <table id="4slist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th style="width:28px" >序号</th>
                    <th style="width:28px"  >目录</th>
                    <th style="width:28px"  >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th style="width:25px"  >BPM</th>
                    <th style="width:40px"  > </th>
                    <th style="width:22px" >EZ</th>
                    <th style="width:22px" >NM</th>
                    <th style="width:22px" >HD</th>
                    <th style="width:26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#4slist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
                ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '4SEZ' },
                    { data: '4SNM' },
                    { data: '4SHD' },
                    { data: '4SSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "5K STANDARD"

    <table id="5slist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th width="28px" >序号</th>
                    <th width="28px" >目录</th>
                    <th width="28px" >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th width="25px" >BPM</th>
                    <th width="40px" > </th>
                    <th width="22px" >EZ</th>
                    <th width="22px" >NM</th>
                    <th width="22px" >HD</th>
                    <th width="26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#5slist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
               ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '5SEZ' },
                    { data: '5SNM' },
                    { data: '5SHD' },
                    { data: '5SSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "6K STANDARD"

    <table id="6slist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th width="28px" >序号</th>
                    <th width="28px" >目录</th>
                    <th width="28px" >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th width="25px" >BPM</th>
                    <th width="40px" > </th>
                    <th width="22px" >EZ</th>
                    <th width="22px" >NM</th>
                    <th width="22px" >HD</th>
                    <th width="26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#6slist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
                ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '6SEZ' },
                    { data: '6SNM' },
                    { data: '6SHD' },
                    { data: '6SSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

=== "8K STANDARD"

    <table id="8slist" class="display" style="width:100%">
            <thead>
                <tr>
                    <th width="28px" >序号</th>
                    <th width="28px" >目录</th>
                    <th width="28px" >图标</th>
                    <th>歌名</th>
                    <th>艺术家</th>
                    <th width="25px" >BPM</th>
                    <th width="40px" > </th>
                    <th width="22px" >EZ</th>
                    <th width="22px" >NM</th>
                    <th width="22px" >HD</th>
                    <th width="26px" >SHD</th>
                </tr>
            </thead>
    </table>
    <script>
        $(document).ready(function () {
            $('#8slist').DataTable({
                // ajax: $.csv.toObjects(require('songlist.csv'));
               ajax: 'songlist.json',
                "pageLength": 25,
                "autoWidth": false,
                columns: [
                    { data: '序号' },
                    { data: '目录' },
                    { data: '图标' },
                    { data: '歌名' },
                    { data: '艺术家' },
                    { data: 'BPM'},
                    { data: 'BPMRNG'},
                    { data: '8SEZ' },
                    { data: '8SNM' },
                    { data: '8SHD' },
                    { data: '8SSHD' },
                ],
                columnDefs: [
                    { orderable: false, targets: [2,6] }
                ],
                order: [[0, 'asc']]
            });
        });
    </script>

<!-- USE BELOW FOR BootStrap Themes, but there seems to be a slight problem with MkDocs Bootstrap... 
<script type="text/javascript" charset="utf8" src="//code.jquery.com/jquery-1.10.2.min.js"></script>
<link rel="stylesheet" type="text/css" href="//cdn.datatables.net/plug-ins/1.10.7/integration/bootstrap/3/dataTables.bootstrap.css">
<script type="text/javascript" charset="utf8" src="//cdn.datatables.net/plug-ins/1.10.7/integration/bootstrap/3/dataTables.bootstrap.js"></script>
-->

