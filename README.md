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

Next we do footprints mapping for the components. For that we remove the simulation components from the schematic and add connectors.  

![Screenshot from 2024-01-05 12-12-13](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/9bbebaee-3883-4b10-8217-27a6736e9927)  

Now go to components to footprint mapping on the top right and assign the footprints as shown and generate the pcb netlist(.net file) fromthe generate netlist on the top right.

![Screenshot from 2024-01-08 12-28-23](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/dd7e4acd-6251-4b9d-85fc-fedbe6470175)  

After which we open the pcb layout design tool from the schematic window on the top right. Next in the layout editor go to read netlist and browse to the .net file generated and select the read current netlist to get the footprints layout. After which arrange the footprints in a way to minimise the lengths of the connections. Then select in tools to lay lines and polygon and selest from the right tab edge.cut and make the PCB edge. Next select tracks or press X and from right tab select B.cu and connect the footprints. Next we need to connect ground fill option from the right and make the groung boundary after which right click inside the boundary and select fill or refill option.  
The following shows the layout:  

![Screenshot from 2024-01-07 16-07-16](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/45592e40-f636-42d5-8910-1a3e158abbab)

This is the DRC report:  

![Screenshot from 2024-01-07 10-20-40](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/de59c516-234f-4b09-a568-f964a0f0dfaa) 

The following shows the gerber file generation and drill file generation.  
![Screenshot from 2024-01-07 10-28-08](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/9fd42298-9dd3-41de-8b5d-973adc1ae4a4)

![Screenshot from 2024-01-07 10-27-41](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/1fb94196-c6f7-4d08-b915-d7671c9f5297)


To view the gerber files go to gerbeview in terminal and open all the files generated.  

![Screenshot from 2024-01-07 10-30-48](https://github.com/Avs-Bharguav/PCB-design-of-Astable-multivibrator/assets/130825917/9515a321-815b-42ba-9ca3-f8c5962ecc90)
