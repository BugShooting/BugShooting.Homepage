---
layout: page
permalink: /releasenotes/
---

<script type="text/javascript">

  const request = new XMLHttpRequest();
    
  request.open("GET", "https://services.bugshooting.com/rest/releasenotes.md");
  
  request.setRequestHeader('Access-Control-Allow-Origin', 'https://services.bugshooting.com');
	request.setRequestHeader('Access-Control-Allow-Credentials: true');
	request.setRequestHeader('Access-Control-Allow-Methods: GET');
  request.setRequestHeader('Access-Control-Allow-Headers: Content-Type');
  
  request.send();

  request.onload = (e) => {
     document.getElementById("releasenotes").textContent = request.response;
  }
  
</script>

# Release Notes

<span id="releasenotes"></span>
