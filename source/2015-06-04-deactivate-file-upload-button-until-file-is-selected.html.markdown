---
title: Deactivate-file-upload-button-until-file-is-selected
date: 2015-06-04 23:12 UTC
tags: js
---

```
$(document).ready(function(){
  $('input:submit').attr('disabled',true);
  $('input:file').change(
      function(){
          if ($(this).val()){
              $('input:submit').removeAttr('disabled');
          }
          else {
              $('input:submit').attr('disabled',true);
          }
      });              
});
```