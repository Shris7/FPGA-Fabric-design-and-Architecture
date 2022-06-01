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
