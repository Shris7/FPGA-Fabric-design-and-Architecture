## OPEN FPGA
- Open source frame work which can be used to quickly generate a fabric for a custom FPGA
![image](https://user-images.githubusercontent.com/92938137/171328740-2491d009-ba88-4a36-bf2c-4246ab4d902f.png)

- VTR Flow
![image](https://user-images.githubusercontent.com/92938137/171329510-235209bf-9c70-4aa6-af38-5e2ba25a705d.png)
- VTR uses an XML based architecture description language to decribe the custom FPGA architecture.

- You can setup your VTR using the link [here](https://docs.verilogtorouting.org/en/latest/quickstart/).
- VTR Flow Results LOG

![image](https://user-images.githubusercontent.com/92938137/171354541-aff7ad06-f54d-4387-9d43-3ca1aeceeb82.png)
- Toggle net

![image](https://user-images.githubusercontent.com/92938137/171363402-7a72a17d-a9bc-4718-9e8c-b62b45e405f4.png)
- Toggle Congested

![image](https://user-images.githubusercontent.com/92938137/171363834-619a2f99-8123-4779-8d23-2d6e8d9b76ff.png)
- Critical Path flyiness Delay

![image](https://user-images.githubusercontent.com/92938137/171364008-5b97a996-12a9-4e3e-8632-a10e4ea013b9.png)

- If you just want the anlysis step:
![image](https://user-images.githubusercontent.com/92938137/171354947-57ce68bf-d2ed-4309-b59d-e27638c17fd1.png)
On Proceed:
![image](https://user-images.githubusercontent.com/92938137/171355392-bf69e97c-61f4-4236-a6d0-4cd41f81f690.png)
- Since no constraints are provided,it shows that the slack is violated
![image](https://user-images.githubusercontent.com/92938137/171357509-83a27e1d-999a-45d0-82e7-5d4dd5822018.png)
- To avoid this we write a .sdc file
![image](https://user-images.githubusercontent.com/92938137/171367534-adaf71a6-3f79-4f69-9518-dfea1ee2960a.png)
![image](https://user-images.githubusercontent.com/92938137/171371274-c5d69573-72b5-4c71-9282-cdd1975b344e.png)
![image](https://user-images.githubusercontent.com/92938137/171371046-3fbd8627-a09e-4a90-b806-d94329449ccf.png)
   - Thus we notice that the slack is positive and is met.
- VTR Script run for counter.v

![image](https://user-images.githubusercontent.com/92938137/171374960-11846eff-df5d-4059-9b17-3acaac0ccfab.png)
![image](https://user-images.githubusercontent.com/92938137/171375206-3f442f17-e1cd-456e-bdb9-cd8599a69ddb.png)

- VTR flow - VPR GUI
![image](https://user-images.githubusercontent.com/92938137/171376123-25e2e205-65ac-4ac3-9c7e-79941b3816ca.png)

- Complete VTR Flow
   -Remove the `--analysis` command
![image](https://user-images.githubusercontent.com/92938137/171377015-b9861c1b-8689-4259-8197-e0f1f580620b.png)
![image](https://user-images.githubusercontent.com/92938137/171377220-7e413141-0ac8-4069-8f3f-d5a7d273aabd.png)

- Generate post implementation netlist
![image](https://user-images.githubusercontent.com/92938137/171377991-69c4a34d-73cf-4b12-9677-1703ff1001f0.png)
![image](https://user-images.githubusercontent.com/92938137/171378153-dfca9e85-5b81-43e8-82da-b544e513ca16.png)

- Post Implementation Netlist simulation
![image](https://user-images.githubusercontent.com/92938137/171592104-e6b93814-4119-41ac-a1df-1d75bfb08bc7.png)

- Timing Analysis
  - With 10ns clock 
![image](https://user-images.githubusercontent.com/92938137/171391274-e0b02553-5f23-4d6c-938c-67873968004f.png)

- Area Analysis
![image](https://user-images.githubusercontent.com/92938137/171391945-34fadcd2-ae3d-4c07-9edc-3653b6320ca9.png)
![image](https://user-images.githubusercontent.com/92938137/171392036-04c0413c-2207-46c3-9f65-b7e49a341a72.png)






