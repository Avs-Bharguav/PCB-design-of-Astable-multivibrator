# PCB-design-of-Astable-multivibrator  
Hey guys here we will be learning PCB design. We will start with schematic drawing and simulation of BJT Astable multivibrator in eSim and then component to footprint mapping, defining design parapeters, layout designing and last creating gerber files and viewing them.

Note: The reference to this is the spokentutorials by IIT Bombay. And i really thanks them for creating such an amazing tool and community.  

The following shows the schematic of astable multivibrator. The library for the components are taken from esim library. You can also use any other like skywater130 pdk.  

![Screenshot from 2024-01-04 12-13-10](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/b1b7b612-09c9-43c5-a5f8-69b5e6bcaaaa)  

Next we do the simpuation. First we generate spice netlist. On the top right go to generate netlist and the select spice and select defaule format. Then go to esim main window and press on convert kicad to spice. The following are some parameters too be set.  

![Screenshot from 2024-01-04 12-13-32](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/9984fdee-c826-4202-bc56-760c040f04a1)

Transient analysis parameters:

![Screenshot from 2024-01-04 12-13-39](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/1d77d6ad-d160-4d48-b45a-7348bcc9d418)

Ngspicesimulation results:

![Screenshot from 2024-01-04 12-12-35](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/2b5b1f3b-4d04-435f-a3ef-9b6db67e278a)
