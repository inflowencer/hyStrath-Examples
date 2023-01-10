<h1 align="center">hyStrath Examples - Rarefied & Hypersonic Flow Cases</h1>
<!-- <hr style="height:1px;" /> -->
<h3 align="center">Collection of examples for the rarefied gas dynamics library <a href="https://github.com/hystrath/hyStrath">hyStrath</a></h3>

![](img/shuttle.png)


## 1. Install hyStrath

* Windows, Linux & MacOS: [https://github.com/inflowencer/hyStrath-Docker](https://github.com/inflowencer/hyStrath-Docker) (recommended)
* Ubuntu-22.04: [https://github.com/hystrath/hyStrath](https://github.com/hystrath/hyStrath)


## 2. Get the Example Collection and Run a Test Case

After successful installation, you can download the example repository and run the *Mach 20 cylinder* test case.

### Docker

1. Clone the repo to the host (into your Windows, Linux or MacOS machine)
   ```sh
   git clone https://github.com/inflowencer/hyStrath-Examples.git ~/hyStrath-Examples
   ```
2. Launch the docker image and copy an example from the host repo to the container:
   ```sh
   docker run hystrath -v /mnt/docker 
   cp -r ~/hyStrath-Examples/examples/viking_mars /mnt/docker/.
   ```

3. Run the simulation
   ```sh
   cd hyStrath-Tests/viking_mars && ./Allrun 8  # Run with 8 cores
   ```

### Ubuntu-22.04

```sh
# Clone the examples
git clone https://github.com/inflowencer/hyStrath-Examples.git ~/hyStrath-Examples

# Launch docker
mkdir -p ~/hyStrath-Tests

# Copy and run an example
cp -r ~/hyStrath-Examples/examples/viking_mars ~/hyStrath-Tests/.
cd hyStrath-Tests/viking_mars
./Allrun 8  # Run with 8 cores
```


2. Change into the `viking_mars/` dir and run the case with your desired number of cores `np`
   ```sh
   ```

3. Postprocess the case 


## List of example cases

### CFD

---

#### [Viking-I Mars reentry](examples/cfd/mach_20_cylinder/)

IMAGE PLACEHOLDER

Reentry of the [ Viking-I capsule ](https://en.wikipedia.org/wiki/Viking_1) into Mars atmosphere.

| Property | Value |
| -------- | -----:|
| Altitude | 30 km |
| Velocity | 3750 m/s |
| Temperature | 150 K |
| Pressure | 10 Pa |
| Density | 1e-3 kg/m3 |
| Kn | 0.002 |
| Composition | 97% CO2, 3% N2 |

---

#### [Mach 20 Cylinder](examples/cfd/70deg_blunted_cone/)

IMAGE PLACEHOLDER

*Short description*

#### [Generic Case](examples/cfd/../genericCase/)

Generic case for setting up reacting and non-reacting `hy2Foam` cases.

### DSMC

#### [70&deg; Blunted Cone](examples/dsmc/70deg_blunted_cone/)

IMAGE PLACEHOLDER

*Short description*

#### [Ion thruster](examples/dsmc/ion_thruster/)

IMAGE PLACEHOLDER

*Short description*