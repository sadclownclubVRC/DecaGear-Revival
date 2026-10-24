# DecaGearVR-Revival
An open project to explore reviving the DecaGear concept: a high-resolution PC VR headset with eye tracking, face tracking, and inside-out tracking. Aiming for affordable, modular hardware with dual 2160×2160 LCDs and a 90–120Hz refresh rate. Looking for VR enthusiasts, hardware engineers, and manufacturers interested in making it a reality.

![image alt](https://github.com/sadclownclubVRC/DecaGearVR-Revival/blob/e886fd5a2397fee3ac0631dae5187889cb979fe7/decagear.png)

Proposed Hardware Components

**Status:** Early-stage concept. Components have not yet been tested together.

### 1. Display System

| Component | Proposed specification | Status |
|---|---|---|
| Left display | Sharp LS029B3SX06A, 2160 × 2160 LCD | Candidate |
| Right display | Sharp LS029B3SX06A, 2160 × 2160 LCD | Candidate |
| Combined resolution | 4320 × 2160 pixels | Target |
| Pixel density | Approximately 1058 PPI | Target |
| Refresh rate | 90 Hz baseline, 120 Hz stretch goal | Requires verification |
| Display drivers | Compatible dual-panel controller and interface electronics | To be sourced |

**Important:** Native 120 Hz operation must be confirmed with the panel supplier.

### 2. Optical System

| Component | Proposed specification | Status |
|---|---|---|
| Left lens | Circular Fresnel-style VR lens | To be sourced |
| Right lens | Matching Fresnel-style VR lens | To be sourced |
| Optical design | Inspired by the original DecaGear headset | Concept |
| Field of view | Approximately 114° diagonal as an initial target | Requires testing |
| IPD adjustment | Mechanically adjustable | To be designed |

The goal is to reproduce the appearance of the original DecaGear lenses while achieving comparable optical performance. Exact replacement lenses have not yet been identified.

### 3. Eye-Tracking System

**Preferred starting point: EyeTrackVR**

| Component | Proposed specification | Status |
|---|---|---|
| Eye cameras | 2 × inward-facing monochrome camera modules | To be selected |
| Camera sensor candidate | OmniVision OV9281 | Candidate; compatibility unverified |
| Illumination | Diffuse near-infrared LEDs compatible with the cameras | Requires optical safety assessment |
| Mounts | Custom 3D-printed camera brackets | To be designed |
| Tracking software | EyeTrackVR or compatible open-source alternative | Existing project |
| Output | Gaze direction and eye movement data | Requires integration |

Resources:
- EyeTrackVR: https://github.com/EyeTrackVR/EyeTrackVR
- EyeTrackVR hardware: https://github.com/EyeTrackVR/EyeTrackVR-Hardware
- EyeTrackVR documentation: https://docs.eyetrackvr.dev

### 4. Facial Expression Tracking

**Preferred starting point: Project Babble**

| Component | Proposed specification | Status |
|---|---|---|
| Face camera | 1 × inward-facing camera covering the lower face | To be selected |
| Sensor candidate | OV2640 camera module with a suitable wide-angle lens | Candidate |
| Field of view | Approximately 120–160° as a sourcing target | Requires verification |
| Lighting | Suitable visible or near-infrared illumination | To be determined |
| Camera mount | Integrated beneath the headset optics | To be designed |
| Tracking software | Project Babble | Existing project |
| Output | Mouth and lower-face expression parameters | Requires integration |

Resources:
- Project Babble: https://github.com/Project-Babble/ProjectBabble
- Camera selection guide: https://docs.babble.diy/docs/diytrackers/partsguide/cameras
- Babble hardware: https://github.com/Project-Babble/BabbleHardware

Project Babble focuses on lower-face expression tracking. Additional hardware and software would be required if broader facial tracking were desired.

### 5. Tracking Software Integration

| Component | Proposed approach | Status |
|---|---|---|
| Eye-tracking processing | EyeTrackVR or compatible alternative | To be integrated |
| Face-tracking processing | Project Babble | To be integrated |
| Combined tracking software | Baballonia / VRCFaceTracking integration where supported | To be tested |
| Target platform | Windows PC VR and VRChat | Goal |

Resources:
- Baballonia: https://github.com/Project-Babble/Baballonia
- VRCFaceTracking: https://docs.vrcft.io/

### 6. Outstanding Engineering Work

- Confirm the display panels are available and obtain datasheets.
- Find compatible Fresnel optical assemblies or commission a custom design.
- Confirm camera sensor, lens, frame-rate and interface compatibility.
- Develop display driver and camera interface electronics.
- Design the headset enclosure and camera mounts.
- Implement calibration and integrate tracking outputs.
- Test image quality, latency, comfort and tracking accuracy.
- Verify infrared illumination safety before any eye-facing use.

## 7. 3D Modelling & Industrial Design

**Looking for a 3D modeller / CAD designer.**

One of the main goals of this project is to recreate a headset with a design that looks **as close as possible to the original DecaGear 1**.

I'm looking for someone experienced in 3D modelling, product design, or CAD who could help create a highly accurate model based on the original DecaGear promotional images and available reference material.

### Design goals
- Reproduce the original headset's overall shape, proportions, curves, and front housing.
- Closely match the original facial interface, lens openings, camera positions, and external details.
- Design the internal layout around the proposed dual LCD panels, Fresnel-style lenses, eye-tracking cameras, and face-tracking camera.
- Make the model suitable for eventual 3D printing and physical prototyping.
- Keep the design modular where possible, allowing components to be replaced or adjusted.

### Desired deliverables
- A detailed 3D model of the exterior.
- A separate internal assembly showing the proposed component layout.
- Editable CAD files or source files, plus STL files for 3D printing where appropriate.

**Important:** The goal is not simply to make a headset inspired by DecaGear. I want to get the design as close to the original as technically and legally possible, while adapting the internals for modern components.

If you're a 3D modeller, CAD designer, or industrial designer interested in collaborating, please get in touch!

### Project Goal

Develop a technically feasible, DecaGear-inspired PC VR headset with dual high-resolution LCD panels, Fresnel-style optics, eye tracking and lower-face tracking.

This parts list is a starting point for discussion and collaboration, not a validated production design. Hardware engineers, optical specialists and VR developers are welcome to contribute suggestions and identify compatible components.
