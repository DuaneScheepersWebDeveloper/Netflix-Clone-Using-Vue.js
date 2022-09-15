<template>
	<header>
		<router-link to="/">
			<h1><span>Vue</span>Netflix Clone App</h1>
		</router-link>
	</header>
	<main>
		<router-view />
	</main>
</template>

<style lang="scss">
* {
	&::selection {
		background: transparentize(#42b883, 0.5);
	}
}

a {
	text-decoration: none;
}

header {
	display: flex;
	align-items: center;
	justify-content: center;
	padding: 10px 16px;
	background-color: #111;
	box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
	border-bottom: 3px solid #42b883;

	h1 {
		color: #fff;
		font-size: 28px;

		span {
			color: #42b883;
		}
	}
}
* {
	font-family: 'Roboto', arial, helvetica, sans-serif;
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
body {
	background-color: #35495e;
	margin: 0;
	position: relative;
}
#content {
	padding-bottom: 20rem;
}
.header {
	display: flex;
}
.logo {
	color: white;
}

span {
	font-weight: 500;
}
.button span {
	cursor: pointer;
	display: inline-block;
	position: relative;
	transition: 0.5s;
}

.button span:after {
	content: '\00bb';
	position: absolute;
	opacity: 0;
	top: 0;
	right: -20px;
	transition: 0.5s;
}

.button:hover span {
	padding-right: 25px;
}

.button:hover span:after {
	opacity: 1;
	right: 0;
}

.header a.logo {
	font-size: 25px;
	font-weight: bold;
}

footer {
	border-top: 3px solid #42b883;

	position: absolute;
	bottom: 0;
	width: 100%;

	background: #111;
	height: 20rem;
	width: 100%;

	padding-top: 40px;
	color: #fff;
}

.footer-content {
	display: flex;
	align-items: center;
	justify-content: center;
	flex-direction: column;
	text-align: center;
}

.footer-content h3 {
	font-size: 2.1rem;
	font-weight: 500;
	text-transform: capitalize;
	line-height: 3rem;
}

.footer-content p {
	max-width: 500px;
	margin: 10px auto;
	line-height: 28px;
	font-size: 14px;
	color: #cacdd2;
}

.socials {
	display: grid;
	grid-template-columns: 1fr 1fr 1fr;
	align-items: center;

	justify-content: center;
}

.socials div {
	padding: 15px;
	justify-content: center;
	text-align: center;
}

.socials a {
	margin-left: -20px;
	display: flex;
	text-decoration: none;
	color: #fff;
	justify-content: center;
	padding: 20px;
	text-align: center;
	border-radius: 100%;
}

.socials a i {
	font-size: 3rem;
	width: 20px;

	transition: color 0.4s ease;
}

.socials a:hover i {
	color: #42b883;
}

.footer-bottom {
	background: #000;
	width: 100%;
	bottom: 0;
	text-align: center;
	border-bottom: 3px solid #42b883;
}
.footer-bottom button {
	float: left;
	margin-top: 10px;
	margin-bottom: 10px;
	padding-left: 20px;
	vertical-align: middle;
	align-items: center;
	justify-content: center;
}

.footer-bottom p a {
	color: #42b883;
	font-size: 16px;
	text-decoration: none;
}

.footer-menu {
	float: right;

	padding-right: 20px;
}

.footer-menu a:hover {
	color: #165237;
}

.footerArrow {
	color: #42b883;
	font-size: 2.1rem;
}

@media (max-width: 500px) {
	.footer-menu {
		display: flex;
	}
}

.icon {
	width: 20rem;
	height: auto;
}

.bottomLine {
	width: 100%;
	color: rgb(255, 255, 255);
	font-size: 14px;
	padding-top: 20px;
	border-top: 2px solid rgb(255, 255, 255);
}
</style>
