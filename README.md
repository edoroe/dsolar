<h2>1. Description</h2>

<p><b>dSolar</b> is a complex of <b>programs and devices</b> for monitoring and managing your solar power plant.
    </p>
    <div class="subparagraphname">dSolar consists of:</div>
    <ul>
      <li><b><u>dSolard</u></b> - the server program for collecting and processing information from equipment sensors.
        <p>
          The dSolard server program runs on OS Linux and can be installed on the:
          <ul>
            <li>
              <b>mini-PC</b> 
              (such as Beelink, Firebat, Soyo, GMKTec, GenMachine, Chuwi, Geekom, Teclast, ...)
            </li>
            <li>
              <b>SBC</b>
              (such as Raspberry PI, Orange PI, Radxa, Odroid, Khadas, Banana PI, ...)
            </li>
            <li>
              <b>Linux Development Board</b>
              (such as Luckfox, Arduino Uno Q, MangoPi, STM32MP1, ...)
            </li>
          </ul>
        </p>
        <p>All data, collected by the server, is stored locally on your Linux device. 
          The data is stored once per second.
        </p>
        <p>dSolard can collect information from sensors of any equipment that supports the Modbus data transfer protocol.
        </p>
        <p>The program has a built-in battery charge management algorithm and calculation SOC.
        </p>
        <p> 
          The program has an energy management mechanism "Energy Control" and "WinterESS" and "DAM (Day Ahead Market)".
        </p>
        <p> 
          Allows you to create rules for controlling additional equipment (inverters, relays, ...) 
          based on sensor values combined with logical operations.
        </p>
        <p>Allows you to track critical system states and report them using "Telegram".
        </p>
        <br>
      </li>
      <li><b><u>dSolar</u></b> - the client program is designed for data visualization.
        <p>
          The dSolar client program runs on a Linux, Windows or Andorid OS.
        </p>
      </li>
    </ul>
    
    <h4>dSolar is not only a software complex, it is a program + device.
    </h4>

    <div class="subparagraphname">Such a monitoring device may look like:</div>
    <ul>
      <li>a USB-stick for connecting via a USB interface to another device, for example, a Victron Cerbo GX</li>
      <li>a USB-dongle for connecting directly to the inverter, for example, to an additional RS485/RS232 Modbus connector</li>
      <li>or, familiar to everyone, a mini-PC or SBC installation</li>
    </ul>
    
    <div class="subparagraphname">dSolar integration:</div>
    <ul>
      <li><a href="#Grafana" title="Grafana">Grafana</a></li>
      <li><a href="#MQTT" title="MQTT">MQTT</a></li>
    </ul>

<h2>2. Examples</h2>
<p>
The examples_dbs directory contains sample databases for various types of hardware.
You need to copy the desired example file to the working directory of the server database. For example:
</p>
<pre>
$ cp AllInOne.dbs dbs/dsolar.dbs
<div>
