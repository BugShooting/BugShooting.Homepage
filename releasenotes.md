---
layout: page
permalink: /releasenotes/
---

<script type="text/javascript">

  const request = new XMLHttpRequest();
    
  request.open("GET", "https://services.bugshooting.com/rest/releasenotes.md");
  request.setRequestHeader('Access-Control-Allow-Headers', 'services.bugshooting.com');
  request.send();

  request.onload = (e) => {
     document.getElementById("releasenotes").textContent = request.response;
  }
  
</script>

# Release Notes

<span id="releasenotes"></span>
