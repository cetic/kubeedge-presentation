# Reveal.js template slides

This repository contains a template for reveal.js presentation slide.

1. Fork this repository
2. Setup CI/CD (project name in `.gitlab-ci` file, Openshift config)
3. Edit `index.html`
4. Edit main title, Authors in README.md

### Usage

Open index.html in your browser or deploy this on OpenShift e.g. (see `.gitlab.yml`)

* presentation mode: press `s`
* overview mode: press `escape`
* pdf/print version: go to http://your_slides_url/?print-pdf#/

See OpenShift usage documentation for deployment instructions: https://git.cetic.be/OpenShift/documentation/tree/master/webconsole/#tldr

Result is here: http://presentation-template.openshift.ext.cetic.be

#### Create a 2 column slide

Using `div`:

```html
<section  data-background-image="img/logo-cetic.png" data-background-position="98% 2%" data-background-size="10%">
	<h2>How to create à double content based slide </h2>
	<div  style="left:-8.33%; text-align: left;  float: left;  width:50%;  z-index:-10;">
		<ul>
			<li>First part of the slide</li>
			<li>Left side of the slide</li>
		</ul>
	</div>
	<div  style="left:31.25%;  top: 75px;  float: right;  text-align: left;  z-index:-10;  width:50%;">
		<ul>
			<li>Second part of the slide</li>
			<li>Right side of the slide</li>
		</ul>
	</div>
</section>
```

Using a `table`:

```html
<table>
	<tr>
		<td style="width: 50%;">bla</td>
		<td>bli</td>
	</tr>
</table>
```

### References

* https://github.com/hakimel/reveal.js/

### Authors

* **Alexandre Nuttinck** : alexandre.nuttinck@cetic.be
* **Sebastien Dupont** : sebastien.dupont@cetic.be
