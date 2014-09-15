---
layout: default
title: textarea
---
<script type="text/javascript">
	document.addEventListener('DOMContentLoaded', function(e){
		document.forms.textinput.addEventListener('keyup', function(e) {
			localStorage.textarea = document.forms.textinput.text.value;
		}, false);
		if(localStorage.textarea){
			document.forms.textinput.text.value = localStorage.textarea;
		} else {
			localStorage.textarea = '';
		}
	}, false);
</script>
<div style="display:flex">
	<form name="textinput">
		<textarea style="width:50%;height:300px" name="text"></textarea>
	</form>
	<div id="preview"></div>
</div>