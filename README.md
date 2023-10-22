# Thermal Statistical Mechanics in Particles Simulation
## Algorithm
- 氣體粒子以點模擬，兩點間短於一定距離即判定碰撞，並施加與相對位置有關的衝量。
- 設 **T** 爲迭代的總步數、 **n** 爲粒子總數。
- 若每迭代都完整檢測所有粒子是否碰撞，則時間複雜度爲 $O(T * n^2)$ ，考慮到距離過遠的粒子間不易發生碰撞，因此採用分成 **m** 區分別計算碰撞的算法來加速，時間複雜度爲 $O(T * \dfrac{n^2}{m})$。
- 定義 **分區精度** 爲 **分區區塊長度** 與 **每迭代的平均粒子位移** 的比值。
- 定義 **碰撞精度** 爲 **平均自由徑** 與 **每迭代的平均粒子位移** 的比值。
- 在保持**分區精度**以及**碰撞精度**的前提下，**T** 與 **n** 成正比，而 **m** 與 $n^3$ 成正比，因此時間複雜度爲 $O(1)$。


## Stimulation Video
The danamic of speed probability distribution of particles trapped in cube/sphere: <br/>
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/89sZ0CZ4Kwc/0.jpg)](https://www.youtube.com/watch?v=89sZ0CZ4Kwc) [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/GO0EKhJZ2n4/0.jpg)](https://www.youtube.com/watch?v=GO0EKhJZ2n4) <br/>

The danamic of speed probability distribution of adiabatic expanding: <br/>
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/f3go-8vIUqg/0.jpg)](https://www.youtube.com/watch?v=f3go-8vIUqg) [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Z1mcMF0FICs/0.jpg)](https://www.youtube.com/watch?v=Z1mcMF0FICs) <br/>

Temperature distribution of particles trapped in long pillar when one side heat up and one side cool down: <br/>
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/sEhC9jxie3I/0.jpg)](https://www.youtube.com/watch?v=sEhC9jxie3I) [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/aa7Ixdy01iU/0.jpg)](https://www.youtube.com/watch?v=aa7Ixdy01iU) <br/>

## Paper
To get the PDF paper click [Thermal_Statistical_Mechanics_in_Particles_Simulation.pdf](Thermal_Statistical_Mechanics_in_Particles_Simulation.pdf)
![image](image/Thermal_Statistical_Mechanics_in_Particles_Simulation_page-1.jpg)
![image](image/Thermal_Statistical_Mechanics_in_Particles_Simulation_page-2.jpg)
![image](image/Thermal_Statistical_Mechanics_in_Particles_Simulation_page-3.jpg)
![image](image/Thermal_Statistical_Mechanics_in_Particles_Simulation_page-4.jpg)
![image](image/Thermal_Statistical_Mechanics_in_Particles_Simulation_page-5.jpg)
