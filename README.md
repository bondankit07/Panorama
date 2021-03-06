# Panorama: Real-time Bird's Eye View of an OpenFlow Network


<h3>Introduction</h3>
Panorama is a lightweight, easy to deploy POX based GUI for obtaining real-time network information in SDN environment. Currently, Panorama is capable of presenting network topology information, per-flow and per-port traffic statistics, aggregate statistics, and data transfer rate for each network link. <br/>

<h3>Please don't forget to cite our paper.</h3>

Ankit Gangwal, Mauro Conti, Manoj Singh Gaur. <br>
PANORAMA: Real-time Bird's Eye View of an OpenFlow Network. <br>
In Proceedings of the 14th IEEE International Conference on Networking, Sensing and Control <br>
(IEEE ICNSC 2017), pages 204-209, Falerna, Calabria, Italy, May 16-18, 2017. <br>
DOI: 10.1109/ICNSC.2017.8000092, ISBN: 978-1-5090-4429-0. <br>

<h3>People</h3>
1. <a href="http://www.math.unipd.it/~gangwal/">Ankit Gangwal</a>, University of Padua, Italy<br/>
2. <a href="http://www.math.unipd.it/~conti/">Prof. Mauro Conti</a>, University of Padua, Italy<br/>
3. <a href="http://www.mnit.ac.in/faculty/profile.php?fid=53">Prof. Manoj Singh Gaur</a>, Malaviya National Institute of Technology, India

<h3>News</h3>
Feb 01, 2017: Our paper "PANORAMA: Real-time Bird's Eye View of an OpenFlow Network" has been accepted at <a href="http://icnsc2017.dimes.unical.it/">IEEE ICNSC 2017.</a>

  <h3>Usage Manual<br/></h3>
  * Copy the project directory under <b>pox [~/pox/ext/]</b></br>
  * You might need to set path to <b>pox.py [pox directory (~/pox/)]</b> in your PATH variable, you may do it through terminal as:<br/>
     <b>$ PATH=$PATH:~/pox/<br/>
     $ export PATH</b>
 
  * <h4> How to start [Manual]</h4>
 * Open a new terminal and run a controller module:<br/>
     <b>$ cd pox<br/>
     $ pox.py forwarding.l2_learning</b>
 
 * Open another terminal and run the monitoring module:<br/>
     <b>$ cd [project working directory i.e. ~/pox/ext/panorama]<br/>
     $ pox.py openflow.of_01 --port=5566 panorama.panorama</b>
 
 * Open another terminal and start a network:<br/>
     <b>$ cd [project working directory i.e. ~/pox/ext/panorama]<br/>
     $ sudo python topology/panorama_mininet.py<br/></b>
     *(You may create your own custom topology as well.)*
 
 * [If a browser window/tab doesn't come up automatically.]<br/>
 Open a browser window/tab and navigate to:<br/>
     <b>http://localhost:8080/</b>
 
  * <h4> How to start [Automatic]<br/></h4>
 * Run the bash script:<br/>
    <b>$ cd [project working directory i.e. ~/pox/ext/panorama]<br/>
     $ bash launch.sh</b>
 
<h3>Screenshots</h3>
 
 <b>Loading<b/>
 ![loading](https://cloud.githubusercontent.com/assets/8746855/20607359/d798e8e4-b277-11e6-9080-072e60460234.png)
 <br/>
 
 <b>Home Tab<b/>
 ![home](https://user-images.githubusercontent.com/8746855/35110292-bc3594ac-fc78-11e7-87bd-984b885d9ad7.png)
 <br/>
 
 <b>N/w Configuration Tab<b/>
 ![topo](https://cloud.githubusercontent.com/assets/8746855/20607361/d79917a6-b277-11e6-86e0-794501e9709f.png)
 <br/>
 
 <b>Port Stat Tab<b/>
 ![port](https://cloud.githubusercontent.com/assets/8746855/20607358/d798c4a4-b277-11e6-85e4-d0edcb2c6a80.png)
 <br/>
 
 <b>Aggregate Stat Tab<b/>
 ![agg](https://cloud.githubusercontent.com/assets/8746855/20607363/d79c4c32-b277-11e6-84f1-4b388975807f.png)
 <br/>
 
 <b>Flow Stat Tab<b/>
 ![flow](https://cloud.githubusercontent.com/assets/8746855/20607362/d7994ae6-b277-11e6-8a7f-c549a5634e64.png)
 <br/>
 
 <b>Data Transfer Rate Tab<b/>
 ![uti](https://cloud.githubusercontent.com/assets/8746855/20607364/d7ae23a8-b277-11e6-86d8-2399d554eb1c.png)
