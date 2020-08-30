# GSoC 2020 Report

/\_ <img src="https://summerofcode.withgoogle.com/static/favicon/favicon-32x32.png" height="17px" /> Google Summer of Code - <img src="https://hepsoftwarefoundation.org/images/hsf_logo_angled.png" height="17px" /> **CERN-HSF** \_\

## Phoenix - Experiment Independent Event Display

Phoenix is a web-based, experiment independent event display framework in JavaScript for visualizing HEP experiment data from multiple experiments. This project focused on major improvements for the Phoenix framework and application.

**Technologies:** TypeScript, Angular, [three.js](http://threejs.org/), [JSROOT](https://root.cern/js/), HTML, SCSS

**Mentors:** Edward Moyse, Riccardo Maria Bianchi

### Important Links

* [**Deployed Application**](https://hepsoftwarefoundation.org/phoenix/)
* [**Project Repository / Code**](https://github.com/HSF/phoenix)
* [**Daily Progress**](https://github.com/9inpachi/progress/tree/master/gsoc2020)
* [**Proposal**](https://drive.google.com/file/d/1x66OR-A5O3wUK2lyfJbdAiLGz_fpG1JO/view)

### Work

_The links below (mostly) contain multiple screenshots and screen captures of the features._

#### - Community Bonding Period -

_04 May 2020 - 01 Jun 2020_

During the community bonding period, I started off by solving some of the existing issues so I could integrate better with the code base and as a part of it documented the entire code and used compodoc to deploy the API documentation.

During this period, I made the following contributions.

* [Info panel for logging application actions](https://github.com/HSF/phoenix/pull/80)
* [Improvement of overlay components](https://github.com/HSF/phoenix/pull/81)
* [Complete API documentation](https://github.com/HSF/phoenix/pull/83)

#### - First Phase -

_01 Jun 2020 - 03 Jul 2020_

I started to code from 30th May 2020.

* [Toggle for wireframing geometries](https://github.com/HSF/phoenix/pull/84)
* [Improvement of geometries](https://github.com/HSF/phoenix/pull/97)  
  Improved the materials of geometries, performance and usage of directional light and flickering bugs
* [Selection of 3D object from collections info panel](https://github.com/HSF/phoenix/pull/98)  
  Options to "Move camera to object" and "Highlight object" from the collections info panel
* [Dynamically get metadata for experiment info](https://github.com/HSF/phoenix/pull/99)
* [Support for CMS experiment](https://github.com/HSF/phoenix/pull/104)  
  Loader for loading event data from ".ig" files
  Complete CMS set up with support for CMS physics objects including MuonChambers
* [RungeKutta](https://github.com/HSF/phoenix/pull/121)  
  Ported RungeKutta propagator to TypeScript for extrapolating tracks
* [Scalable Jets and fix depthTest](https://github.com/HSF/phoenix/pull/107)
* Debug and discover issue of why antialiasing was not working

#### - Second Phase -

_03 Jul 2020 - 31 Jul 2020_

* Proposed a new event data JSON format and write conversion functions  
  (Dropped because the proposed format was not good enough)
* [Generalize 'lookAtObject'](https://github.com/HSF/phoenix/pull/109)  
  Improvement of the "Move camera to object" code
* [Loading data of all events in CMS](https://github.com/HSF/phoenix/pull/110)  
  Make events loaded from ".ig" file available in the event selection dropdown of UI menu
* [New Phoenix Menu aka Experiment Controls](https://github.com/HSF/phoenix/pull/112)  
  Custom Phoenix menu for controlling geometry and event data
* [Option to load geometry on demand](https://github.com/HSF/phoenix/pull/114)
* [Fix geometries not repopulating in phoenix menu](https://github.com/HSF/phoenix/pull/115)
* [JSROOT support](https://github.com/HSF/phoenix/pull/117)  
  Support for loading event data from ".root" files through the `JSRootEventLoader`  
  Support for loading detector geometries from ".root" and ".json.gz" files
* Converter for converting locked JSON geometries to glTF for use in Phoenix

#### - Third / Final Phase -

_31 Jul 2020 - 31 Aug 2020_

* [Unit tests](https://github.com/HSF/phoenix/pull/118)  
  Improved code coverage from 62% to 90%!  
  Wrote 150+ unit test specs  
  Fixed already existing tests  
  Upgrade testing packages (jasmine, karma and other related packages)
* [Keyboard controls](https://github.com/HSF/phoenix/pull/119)
* [Major fixes for mobile devices](https://github.com/HSF/phoenix/pull/120)  
  Fixed major bugs making it hard to use Phoenix on mobile devices  
  Added object selection for mobile devices
* [Event animations](https://github.com/HSF/phoenix/pull/129)  
  Toggle to animate and translate camera through the scene  
  Toggle to animate the propagation of event data when two particles collide  
  Option to use spherical shaped clipping planes or individual event data extrapolation for animation
* [Complete VR support](https://github.com/HSF/phoenix/pull/131)  
  Fix VR not working  
  Create a custom toggle for VR (not using the three.js VRButton)  
  Position VR camera where the camera is when the user enters VR mode  
  Support for moving through the event display scene using the VR controller
* Create `AnimationsManager`, `EffectsManager` and `VRManager` for modular code and improve Three and Eventdisplay services

### What's Next

* Detailed documentation on how to use Phoenix as an API to set up any experiment
* Support for loading events from server
* Support for loading TGeo and Geant4 geometries
* More immersive and dedicated VR experience as the WebXR API gets updated
* Support for more experiments

### Remarks

It was a very fun and exciting experience working on Phoenix. I was interested in Phoenix from the last year and had been trying to contribute to it before. Through GSoC, I got the chance to fully commit to it and make some major improvements.

#### Mentors

Edward throughout the project was very helpful and appreciative of the work and always ready to discuss whatever I had in mind. It was a very fruitful experience working on this with him. I hope to be in touch with him and make some major contributions to Phoenix in the future as well.
