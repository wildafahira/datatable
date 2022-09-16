# datatable
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Latihan 1</title>
    <link rel="stylesheet" href="DataTables/datatables.min.css">
</head>
<body>
    <table id="contoh" class="table table-striped table-bordered">
        <thead>
            </tr>
                <th width="5%">No</th>
                <th width="50%">Nama</th>
                <th width="15%">Kelas</th>
                <th width="15%">Alamat</th>
                <th width="15%">No Hp</th>
            </tr>
        </thead>
    </table>
<script src="DataTables/jQuery-3.6.0/jquery-3.6.0.min.js"></script>
<script src="DataTables/datatables.min.js"></script>
<script>
        $(function(){
            //var data = [
            //               ["1", "wilda fahira", "XII RPL 1", "kp.cikurutug", "085721368680"],
            //                ["2", "wilda fahira meistria", "XII RPL 1", "kp.cikurutug", "085721368680"],
            //            ];

            var data = [];

            for (let i = 0; i < 5; i++) {
                data.push([i]);
                for (let j = 0; j < 5; j++) {
                    data[i].push(j);
                }
            }
            $("#contoh").DataTable({
                responsive : true,
                data: data
            });
        });
    </script>
</body>
</html>
