# What is *speed-viz*?
*speed-viz* is a visualization tool for data collected by the [Ookla Internet Speed Test](https://www.speedtest.net/) team. Currently, *speed-viz* takes county-level data from the U.S. Census Bureau Tables to create a comparative visualization of internet speed and median income in the state of Virginia. *speed-viz* is intended as a proof-of-concept and technology showcase, and is built on a full stack of modern technologies.

# Stack Structure & Technologies
*speed-viz* is mainly an interactive map that correlates internet speed and median income using linear regression powered by *numpy*. The website leverages the common MERN web development framework:
- **MongoDB** database to host [Ookla's dataset](https://registry.opendata.aws/speedtest-global-performance/)
- **Node.js** + **Express.js** to build the application layer
- **React.js** to build the interactive UI.
- **Python** to perform regression on the raw data
- **Amazon EC2** running Ubuntu to power the stack
