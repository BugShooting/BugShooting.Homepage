---
layout: page
permalink: /releasenotes/
---

<script type="text/javascript">

  const request = new XMLHttpRequest();
    
  request.open("GET", "https://services.bugshooting.com/rest/releasenotes.md");
  request.send();

  request.onload = (e) => {
     document.getElementById("releasenotes").innerHTML = request.response;
  }
  
</script>

# Release Notes

<div id="releasenotes" />
