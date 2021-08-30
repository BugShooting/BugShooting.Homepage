---
layout: page
permalink: /releasenotes/
---

<script type="text/javascript">

  const response = new XMLHttpRequest();
  response.open("GET", "https://services.bugshooting.com/rest/releasenotes.md");
  response.send();

  response.onload = (e) => {
     document.getElementById("releasenotes").textContent = response.response)
  }
  
</script>

# Release Notes

<span id="releasenotes"></span>
