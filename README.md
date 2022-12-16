<h1 align="center">hyStrath Examples - Rarefied & Hypersonic Flow Cases</h1>
<!-- <hr style="height:1px;" /> -->
<h3 align="center">Collection of examples for the rarefied gas dynamics library <a href="https://github.com/hystrath/hyStrath">hyStrath</a></h3>

![](img/shuttle.png)


### Install hyStrath

* Ubuntu-22.04: [https://github.com/hystrath/hyStrath](https://github.com/hystrath/hyStrath)
* Windows, Linux & MacOS: [https://github.com/inflowencer/hyStrath-Docker](https://github.com/inflowencer/hyStrath-Docker)


### Get the Example Collection

```sh
git clone https://github.com/inflowencer/hyStrath-Examples.git ~/hyStrath-Examples
```

### Run the Mach 20 Cylinder Test Case

1. With **docker**, run/mount the container and copy the test case into it
   ```sh
   docker run hystrath -v /mnt/docker 
   cp -r ~/hyStrath-Examples/examples/viking_mars /mnt/docker/.
   ```
   With **Ubuntu**, create a new directory and copy the test case from the repo inside it
   ```sh
   mkdir -p ~/hyStrath-Tests
   cp -r ~/hyStrath-Examples/examples/viking_mars ~/hyStrath-Tests/.
   ```

2. Change into the `viking_mars/` dir and run the case with your desired number of cores `np`
   ```sh
   cd hyStrath-Tests/viking_mars
   ./Allrun 8  # Run with 8 cores
   ```

3. Postprocess the case 


## List of example cases

### CFD

#### [Viking-I Mars reentry](examples/dsmc/70deg_blunted_cone/)

IMAGE PLACEHOLDER

*Short description*

#### [Mach 20 Cylinder](examples/dsmc/70deg_blunted_cone/)

IMAGE PLACEHOLDER

*Short description*

### DSMC

#### [70&deg; Blunted Cone](examples/dsmc/70deg_blunted_cone/)

IMAGE PLACEHOLDER

*Short description*

#### [Ion thruster](examples/dsmc/ion_thruster/)

IMAGE PLACEHOLDER

*Short description*