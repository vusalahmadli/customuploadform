# customuploadform
Custom upload input feld.

HTML:


<div class="input-group mb-2 mt-3 col-12">
  <div class="custom-file">
    <input type="file" class="custom-file-input" id="anschreiben" style="opacity: 0">
    <label class="custom-file-label w-100 p-2 bg-white" style="border-radius: 0; border: 1px solid #ced4da" id="label_anschreiben" for="anschreiben">Laden Sie hier Ihren Kassenbon hoch*</label>
  </div>
</div>




JQuery:

<script>
  $('#anschreiben').on('change', function() {
    var filePath = $(this).val();
      var fileName = filePath.replace("C:\\fakepath\\", "");
      if (fileName) {
                  $('#label_anschreiben').text(fileName);
    }
  });
</script>



