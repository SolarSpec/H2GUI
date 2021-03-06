<div id="top"></div>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/SolarSpec/H2GUI">
    <img src="H2_Fitting_resources/logo.png" alt="SolarSpec" width="160" height="120">
  </a>

<h3 align="center">H2 Evolution GUI</h3>

  <p align="center">
    A Graphical User Interface 
    <br />
    <a href="https://github.com/SolarSpec/H2GUI"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/SolarSpec/H2GUI">View Demo</a>
    ·
    <a href="https://github.com/SolarSpec/H2GUI/issues">Report Bug</a>
    ·
    <a href="https://github.com/SolarSpec/H2GUI/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![H2 Screenshot][product-screenshot]](https://solarspec.ok.ubc.ca/)

Similar to the Log-Log Fitting app attached to the Spectrabuilder GUI but instead used for H2 evolution data.

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [MATLAB](https://www.mathworks.com/products/matlab.html)
* [TDMS Reader Addon](https://www.mathworks.com/matlabcentral/fileexchange/30023-tdms-reader)
* [Image Processing Toolbox](https://www.mathworks.com/help/images/)
* [Curve Fitting Toolbox](https://www.mathworks.com/help/curvefit/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To begin using this app is very simple. Just verify you have the necessary prequisites and follow the installation instructions.

### Prerequisites

Make sure MATLAB is installed. It is available for download in the Software Distribution section under the Help tab after you log into [Canvas.](https://canvas.ubc.ca/)
Click on the "Add-Ons" dropdown menu of your MATLAB Home screen. Then click on "Manage Add-Ons" and ensure you have the Image Processing Toolbox and the Signal Processing Toolbox. If not, click on "Get Add-Ons" button instead and search for the aforementioned products.


### Installation

1. Clone the repo to your PC
   ```sh
   git clone https://github.com/SolarSpec/H2GUI.git
   ```
2. Install the application 
   ```
   Click on the .mlappinstall file in your repository to open and install in MATLAB
   ```
3. Browse the APPS header
   ```
   You will find the recently installed application and can add it to your favourites
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

To begin, load some H2 evolution data from an excel file (.csv or .xlsx) which will then plot the processed concentration vs. time (s) if it is present in the file. If not, the GUI will revert to the raw data which displays voltage (mV) vs. time (s). In this case you can manually input the slope and intercept values of the linear equation that relates the raw to the processed concentration data. There is also an edit field for the volume in (mL) that multiplies the processed data by the inputted value to convert it into moles (nmol). 

There are fields to edit the fit limits which change the position of the ROI lines overlaying the data. Changing these values allow you to partition the data in order to save specific slopes to the table on the left panel. The user can repeat this process as many times as desired while also changing the units and even resetting the table if needed. At the bottom of the left panel displays the mean and standard deviation of the checked/selected slopes. It is advised to only have the same type of units selected to avoid any issues with the mean values mentioned above. The axes limit fields instead crops the plot data and exported data by the inputted values.

_For more information on data filtering and decimation, please refer to the [Documentation](https://www.mathworks.com/help/signal/ref/decimate.html#d123e21788)_

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [X] Plot H2 evolution data
- [X] Calculate fit of certain time slices
- [X] Save the slopes of each slice
    - [X] Reset table data
- [X] Calculate respective mean and std. dev of selected saves
- [X] Vary data scale if present in loaded file
    - [X] Calculate generated plot or processed data

See the [open issues](https://github.com/SolarSpec/H2GUI/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the BSD 3-Clause License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

SolarSpec - [SolarSpec Website](https://solarspec.ok.ubc.ca/) - vidihari@student.ubc.ca

Project Link: [https://github.com/SolarSpec/H2GUI](https://github.com/SolarSpec/H2GUI)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Group Leader - Dr. Robert Godin](https://solarspec.ok.ubc.ca/people/)
* [Group Alumni - James Kivai](https://solarspec.ok.ubc.ca/people/)
* [The Entire SolarSpec Team](https://solarspec.ok.ubc.ca/people/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/SolarSpec/H2GUI.svg?style=for-the-badge
[contributors-url]: https://github.com/SolarSpec/H2GUI/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/SolarSpec/H2GUI.svg?style=for-the-badge
[forks-url]: https://github.com/SolarSpec/H2GUI/network/members
[stars-shield]: https://img.shields.io/github/stars/SolarSpec/H2GUI.svg?style=for-the-badge
[stars-url]: https://github.com/SolarSpec/H2GUI/stargazers
[issues-shield]: https://img.shields.io/github/issues/SolarSpec/H2GUI.svg?style=for-the-badge
[issues-url]: https://github.com/SolarSpec/H2GUI/issues
[license-shield]: https://img.shields.io/github/license/SolarSpec/H2GUI.svg?style=for-the-badge
[license-url]: https://github.com/SolarSpec/H2GUI/blob/main/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/haris-vidimlic-06730019b/
[product-screenshot]: H2_Fitting_resources/Screenshot.png
