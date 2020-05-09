<!DOCTYPE html>
<html lang="en">
	<!-- Head -->
	{% include head.html %}
	
<body>
	<div id="fh5co-wrapper">
	<div id="fh5co-page">
	<!-- Header -->
	{% include header.html %}
	<!-- Page content -->
	<div class="fh5co-parallax" style="background-image: url({{ "/assets/img/home-image.jpg" | relative_url }});" data-stellar-background-ratio="0.5">
		<div class="overlay"></div>
		<div class="container">
			<div class="row">
				<div class="col-md-8 col-md-offset-2 col-sm-12 col-sm-offset-0 col-xs-12 col-xs-offset-0 text-center fh5co-table">
					<div class="fh5co-intro fh5co-table-cell animate-box">
						<h1 class="text-center">{{ page.title }}</h1>
						<p>{{ page.description }}</p>
					</div>
				</div>
			</div>
		</div>
	</div>
	<!-- end: fh5co-parallax -->
	<!-- end:fh5co-hero -->
	<div id="fh5co-team-section">
		<div class="container">
			<div class="row">
				<div class="col-md-12 col-md-offset-0 animate-box">
					{%- if page.quote -%}
					<blockquote><p>{{ page.quote }}</p></blockquote>
					{%- endif -%}
					<p>{{ content }}</p>
				</div>
			</div>
		</div>
	</div>
	<!-- Footer -->
	{% include footer.html %}
	</div>
	<!-- END fh5co-page -->
	</div>
	<!-- END fh5co-wrapper -->

<!-- Scripts-->
{% include scripts.html %}

</body>
</html>