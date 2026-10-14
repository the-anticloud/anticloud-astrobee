# ASTROBEE

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-space_aerotech-lightgrey)

> Anticloud-hardened packaging of the upstream project `ASTROBEE` in category **SPACE AEROTECH**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SPACE AEROTECH · **Upstream:** https://github.com/nasa/astrobee · **Upstream pin:** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# Astrobee Robot Software

### About

<img src="doc/images/astrobee.png" srcset="../images/astrobee.png 1x"
  title="Astrobee" align="right" style="display: inline"/>
Three NASA [Astrobee free-flying robots](https://nasa.gov/astrobee/) have been operating inside
the International Space Station (ISS) since 2019. This [`astrobee`](https://github.com/nasa/astrobee) project contains source code for the Astrobee Robot Software, consisting of
the flight software that runs onboard the Astrobee robots, a software simulator, and supporting tools, primarily written in C++.

Astrobee's flight software performs vision-based localization,
provides autonomous navigation, docking and perching, manages various sensors
and actuators, and supports human-robot interaction with co-located astronauts via screen-based displays, light
signaling, and sound. The flight software is hosted on each Astrobee's three internal single board computers and
uses the open-source [Robot Operating System (ROS)](https://www.ros.org/) framework as message-passing
middleware.  It provides a high-level [Astrobee Command API](https://nasa.github.io/astrobee/html/command_dictionary.html) for controlling the robot and has multiple operating modes. It can execute a plan (command sequence), individual operator commands (teleoperation), or commands from guest science code running onboard Astrobee.

The Astrobee Robot Software simulator, built using [ROS](https://www.ros.org/) and [Gazebo](http://gazebosim.org/), enables the flight software to be evaluated without the need for robot hardware. The supporting tools include a tool that processes ISS imagery to [build maps for Astrobee localization](https://nasa.github.io/astrobee/html/sparsemapping.html), along with many others.

Released separately, the Astrobee ground data system (GDS) includes Astrobee control station software that communicates with Astrobee flight software via the Data Distribution Service (DDS) network protocol over the ISS Ku-IP space-to-ground link. The control station is written primarily in Java using the Eclipse RCP framework. Source code is in the [`astrobee_gds`](https://github.com/nasa/astrobee_gds) project, or you can download the [binary release](https://software.nasa.gov/software/ARC-17994-1B).

Together, the Astrobee Robot and Ground Software were the NASA Software of the Year Award Runner-Up in 2020!

The Astrobee Robot Software remains a work in progress. Please consult the
[release notes](https://nasa.github.io/astrobee/html/md_RELEASE.html) for the current list of features and limitations.

### Usage

[Instructions on installing and using the Astrobee Robot Software](https://nasa.github.io/astrobee/html/md_INSTALL.html).

### Contributing

The Astrobee Robot Software is open source, and we welcome contributions
from the public. Please submit pull requests to the [`develop`](https://github.com/nasa/astrobee/tree/develop) branch. The code must follow the [Astrobee code style](https://nasa.github.io/astrobee/html/astrobee-code-style.html).
For us to merge any pull requests, we must request that contributors sign and submit a
[Contributor License Agreement](https://www.nasa.gov/sites/default/files/atoms/files/astrobee_individual_contributor_license_agreement.pdf)
due to NASA legal requirements. Thank you for your understanding.

### Documentation

[Extensive documentation is auto-generated from the contents of this project.](https://nasa.github.io/astrobee/documentation.html)

["A Brief Guide to Astrobee’s Flight Software"](https://github.com/albee/a-brief-guide-to-astrobee/raw/master/a_brief_guide_to_astrobee_latest.pdf) is a good tutorial, with a particular emphasis on the advanced topic of modifying Astrobee's flight software to enable Guidance, Navigation, & Control (GN&C) research. (Note that most guest science can be implemented as an app that uses the [Astrobee Command API](https://nasa.github.io/astrobee/html/command_dictionary.html) without modifying the flight software.)

The ["Astrobee ROS Demo"](https://github.com/Pedro-Roque/astrobee_ros_demo) package provides a C++/Python interface to implement custom control methods in ROS.

For more information, read [Astrobee-related publications](https://www.nasa.gov/astrobee-research-publications/).
Learning about the Astrobee [platform](https://ntrs.nasa.gov/api/citations/20160007769/downloads/20160007769.pdf),
[software](https://brian.coltin.org/pub/fluckiger2018astrobee.pdf), [original mapping and localization system](https://www.nasa.gov/sites/default/files/atoms/files/coltin2016localization.pdf), and [current localizer](https://ntrs.nasa.gov/api/citations/20250001870/downloads/astroloc2_final.pdf)
are good starting points.

### Guest Science

The ISS Astrobee Facility maintains a collection of [resources for guest scientists](https://www.nasa.gov/content/guest-science-resources) interested in conducting research with Astrobee, including the [Astrobee Guest Science Guide](https://www.nasa.gov/sites/default/files/atoms/files/irg-ff029-astrobee-guest-science-guide.pdf) overview.

Guest science code that runs onboard Astrobee is usually hosted as an Android Java app running on Astrobee's high-level processor (HLP). Guest science apps can use the [Astrobee Command API](https://nasa.github.io/astrobee/html/command_dictionary.html) through its Java bindings. The [`astrobee_android`](https://github.com/nasa/astrobee_android) project contains source code for Astrobee services that run on the HLP, example guest science apps, as well as a [Guest Science Readme](https://github.com/nasa/astrobee_android/blob/master/guest_science_readme.md) and [Guest Science Developer Guide](https://github.com/nasa/astrobee_android/blob/master/gs_developer_guide.md) focused on HLP guest science apps.

### License

Copyright (c) 2017, United States Government, as represented by the
Administrator of the National Aeronautics and Space Administration.
All rights reserved.

The Astrobee platform is licensed under the Apa

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `astrobee/`, `behaviors/`, `cmake/`, `communications/`, `debian/`, `description/`, `doc/`, `external/`, `gnc/`, `hardware/`, `localization/`, `management/`
- Snapshot size: **2664 files**, **208880 lines of code** (measured; see Benchmarks)
- Primary languages: `.cc` (473), `.h` (462), `.xml` (169), `(none)` (146), `.md` (142), `.msg` (121)
- Upstream commit pinned for this packaging: `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`

---

## Installation

Released separately, the Astrobee ground data system (GDS) includes Astrobee control station software that communicates with Astrobee flight software via the Data Distribution Service (DDS) network protocol over the ISS Ku-IP space-to-ground link. The control station is written primarily in Java using the Eclipse RCP framework. Source code is in the [`astrobee_gds`](https://github.com/nasa/astrobee_gds) project, or you can download the [binary release](https://software.nasa.gov/software/ARC-17994-1B).

Together, the Astrobee Robot and Ground Software were the NASA Software of the Year Award Runner-Up in 2020!

The Astrobee Robot Software remains a work in progress. Please consult the
[release notes](https://nasa.github.io/astrobee/html/md_RELEASE.html) for the current list of features and limitations.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

[Instructions on installing and using the Astrobee Robot Software](https://nasa.github.io/astrobee/html/md_INSTALL.html).

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The Astrobee Robot Software simulator, built using [ROS](https://www.ros.org/) and [Gazebo](http://gazebosim.org/), enables the flight software to be evaluated without the need for robot hardware. The supporting tools include a tool that processes ISS imagery to [build maps for Astrobee localization](https://nasa.github.io/astrobee/html/sparsemapping.html), along with many others.

Released separately, the Astrobee ground data system (GDS) includes Astrobee control station software that communicates with Astrobee flight software via the Data Distribution Service (DDS) network protocol over the ISS Ku-IP space-to-ground link. The control station is written primarily in Java using the Eclipse RCP framework. Source code is in the [`astrobee_gds`](https://github.com/nasa/astrobee_gds) project, or you can download the [binary release](https://software.nasa.gov/software/ARC-17994-1B).

Together, the Astrobee Robot and Ground Software were the NASA Software of the Year Award Runner-Up in 2020!

The Astrobee Robot Software remains a work in progress. Please consult the
[release notes](https://nasa.github.io/astrobee/html/md_RELEASE.html) for the current list of features and limitations.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 2664 |
| Lines of code | 208880 |
| Dependency references | 301 |
| Dependencies by ecosystem | native: 301 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| native | catkin2 | - | tools/performance_tester/CMakeLists.txt |
| native | catkin | - | tools/localization_rviz_plugins/CMakeLists.txt |
| native | pcl_conversions | - | tools/localization_rviz_plugins/CMakeLists.txt |
| native | Qt5 | - | tools/localization_rviz_plugins/CMakeLists.txt |
| native | catkin | - | tools/localization_rviz_plugins/CMakeLists.txt |
| native | catkin2 | - | tools/localization_analysis/CMakeLists.txt |
| native | GTSAM | - | tools/localization_analysis/CMakeLists.txt |
| native | rostest | - | tools/localization_analysis/CMakeLists.txt |
| native | catkin2 | - | tools/interactive_marker_teleop/CMakeLists.txt |
| native | catkin | - | tools/interactive_marker_teleop/CMakeLists.txt |
| native | catkin | - | tools/gnc_visualizer/CMakeLists.txt |
| native | catkin | - | tools/gds_helper/CMakeLists.txt |
| native | catkin | - | tools/gds_helper/CMakeLists.txt |
| native | Boost | - | tools/gds_helper/CMakeLists.txt |
| native | catkin | - | tools/gds_helper/CMakeLists.txt |
| ... | (286 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `.isort.cfg`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `ASTROBEE` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: Apache-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text

                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `ASTROBEE` (category: SPACE AEROTECH)
- **Upstream URL:** https://github.com/nasa/astrobee
- **Pinned commit (SHA):** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`
- **Branch:** master
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`ecd31e5afc73b428d3ff1eebde9493559b7cdbbcdfa45085b485c44e0886de8e`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

