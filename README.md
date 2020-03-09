<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>vagrantglpi</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><p>Aguyon<br>
<a href="https://twitter.com/aguyonp"><img src="https://img.shields.io/twitter/url?color=blue&amp;label=Twitter&amp;logo=blue&amp;logoColor=blue&amp;style=for-the-badge&amp;url=https://twitter.com/aguyonp" alt="enter image description here"></a> <a href="https://aguyon.net"><img src="https://img.shields.io/twitter/url?color=orange&amp;label=Website&amp;logo=blue&amp;logoColor=blue&amp;style=for-the-badge&amp;url=https://aguyon.net" alt="enter image description here"></a></p>
<h1 id="vagrant-deploye-glpi-instance-on-virtualbox">Vagrant deploye GLPI instance on virtualbox</h1>
<p><img src="https://www.morot.fr/wp-content/uploads/2019/01/vagrant-logo.png" alt="Résultat de recherche d'images pour &quot;vagrant&quot;"><br>
This project makes it possible to deploy a virtualbox <strong>Debian 10</strong> virtual machine with a <strong>GLPI</strong> instance.<br>
The project uses <strong>docker</strong> and <strong>docker-compose</strong> technologies.</p>
<h2 id="prerequisite">Prerequisite</h2>
<p>Install:</p>
<ul>
<li>Virtualbox  <a href="https://www.virtualbox.org/wiki/Downloads">Downloads link</a></li>
<li>Vagrant <a href="https://www.vagrantup.com/downloads.html">Downloads link</a></li>
</ul>
<h2 id="deploying-the-project">Deploying the project</h2>
<ol>
<li>Download archive on github</li>
<li>Open CMD as administrator</li>
<li>Go to “vagrant file” location</li>
<li>Make <code># vagrant up</code></li>
</ol>
<p><img src="https://i.imgur.com/sidYJfl.png" alt="enter image description here"></p>
<p>Vagrant then asks you how many network cards you want.<br>
Only one in the example<br>
<img src="https://i.imgur.com/tR6NHhQ.png" alt="enter image description here"></p>
<p>Let Vagrant configure the VM. Once finished, Vagrant will display a message containing the connection information to GLPI (This may take some time depending on your connection speed).<br>
<img src="https://i.imgur.com/7Fdh8fu.png" alt="enter image description here">The password is generated randomly.</p>
<h2 id="configuration-of-glpi">Configuration of GLPI</h2>
<p>Go to the web page indicated by Vagrant (<a href="http://10.89.1.141">http://10.89.1.141</a>) LAN IP</p>
<p>Follow the configuration steps<br>
Once you have reached the database configuration, enter the information provided by Vagrant, as shown in the following scheme:<br>
<img src="https://i.imgur.com/xPFCU2U.png" alt="enter image description here"><br>
Select this database:<br>
<img src="https://i.imgur.com/muay8yu.png" alt="enter image description here"></p>
<p>GLPI is now operational (Identifiers: glpi / glpi):<br>
<img src="https://i.imgur.com/49K1HzN.png" alt="enter image description here"></p>
</div>
</body>

</html>
