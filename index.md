<!DOCTYPE html>
<html>
<head>
	<title>Select2 - jQuery</title>
	<!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <link rel="shortcut icon" href="assets/img/lp3i_icon.ico">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link href="assets/fontawesome-free/css/all.min.css" rel="stylesheet" type="text/css">

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

	<script src="https://code.jquery.com/jquery-3.4.1.js"></script>
</head>
<body>

<div class="container mt-5">
	<div class="row">
		<div class="col-md">
			<div class="form-group">
				<h4>Select2</h4>
				<label>Nama Barang</label>
				<select class="form-control" id="selectbrg">
					<option value="">--Select Barang--</option>
					<option value="Laptop">Laptop</option>
					<option value="Mouse">Mouse</option>
					<option value="Keyboard">Keyboard</option>
				</select>
			</div>
		</div>

		<div class="col">
			<div class="form-group">
				<h4>Multiple Select</h4>
				<label>Nama Barang</label>
				<select class="form-control" id="multiple" multiple="multiple">
					<option value="">--Select Barang--</option>
					<option value="Laptop">Laptop</option>
					<option value="Mouse">Mouse</option>
					<option value="Keyboard">Keyboard</option>
				</select>
			</div>
		</div>
	</div>
</div>

<link href="https://cdn.jsdelivr.net/npm/select2@4.1.0-beta.1/dist/css/select2.min.css" rel="stylesheet" />
<script src="https://cdn.jsdelivr.net/npm/select2@4.1.0-beta.1/dist/js/select2.min.js"></script>

<script>
	$("#selectbrg").select2();
	$("#multiple").select2({
		placeholder: 'select barang',
		maximumSelectionLength: 2
	});
</script>

</body>
</html>
