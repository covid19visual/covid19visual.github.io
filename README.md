<html>
<head>
<script data-ad-client="ca-pub-6588502553669538" async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<script async src="https://www.googletagmanager.com/gtag/js?id=G-7VMH5QLNQJ"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-7VMH5QLNQJ');
</script>
<script>

	function onSelectionChanged() {
		
		var selection = document.getElementById("selection").value;
		if (selection == "cases") {
			document.getElementById("container").innerHTML = document.getElementById("cases").innerHTML;
		} else {
			document.getElementById("container").innerHTML = document.getElementById("deaths").innerHTML;
	  }
	}
</script>
<style>
	select { font-size: 1.4em; }
</style>
</head>
<body style="text-align:center; font-family: Helvetica, sans-serif" onload="onSelectionChanged()">

<a href="https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases">Data source</a> | <a href="https://forms.gle/ixD1PwoXyzVmUhMt8">Contact</a>
<br />
<br />

<select id="selection" onchange="onSelectionChanged()">
	<option value="cases" selected>Daily new confirmed COVID-19 cases per 100,000 people (rolling 7-day average)</option>
	<option value="deaths">Daily new confirmed COVID-19 deaths per 100,000 people (rolling 7-day average)</option>
</select>

<div id="container"></div>

<div id="cases" style="display:none">
	<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/5280884">
		<script src="https://public.flourish.studio/resources/embed.js"></script>
	</div>
</div>

<div id="deaths" style="display:none">
	<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/5287904">
		<script src="https://public.flourish.studio/resources/embed.js"></script>
	</div>
</div>

</body>
</html>
