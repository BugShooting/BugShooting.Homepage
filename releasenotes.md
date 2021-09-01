---
layout: page
permalink: /releasenotes/
---

<script type="text/javascript">

  const request = new XMLHttpRequest();
    
  request.open("GET", "https://services.bugshooting.com/rest/releasenotes.html");
  request.send();

  request.onload = (e) => {
     document.getElementById("releasenotes").innerHTML = request.response;
  }
  
</script>

# Release Notes

<div id="releasenotes">
  <div style="height:800px">Loading...</div>
</div>
