# CMIP6Plus Controlled Vocabularies

Core Controlled Vocabularies (CVs) for use in CMIP6Plus
#



<div align="center" style="width:100%">
    <img width='180px' style='fill:red;' src='https://raw.githubusercontent.com/WCRP-CMIP/CMIP6Plus_CVs/main/.github/.wiki/CMIP6plus.svg'/>
   <br>
    <table>
        <tr>
            <td><strong>Description</strong></td>
            <td>
            <a href='https://github.com/WCRP-CMIP/CMIP6Plus_CVs/releases'><img src='https://img.shields.io/github/release/WCRP-CMIP/CMIP6Plus_CVs?label=CV%20Version%20%5Blatest%5D'></a>
            <a href='https://github.com/PCMDI/cmor'><img src='https://img.shields.io/github/release/PCMDI/cmor?label=CMOR%20Version&color=green'></a>
            <a href='https://github.com/PCMDI/mip-cmor-tables'><img src='https://img.shields.io/github/release/PCMDI/mip-cmor-tables?label=MIP%20Table%20Version&color=purple'></a>
            <img src='https://img.shields.io/github/license/WCRP-CMIP/CMIP6Plus_CVs.svg'/>
            </td>
        </tr>
        <tr>
            <td><strong>Repository Status</strong></td>
            <td><img src='https://github.com/WCRP-CMIP/CMIP6Plus_CVs/actions/workflows/gen_CV.yml/badge.svg?branch=main'>
            <img src='https://github.com/WCRP-CMIP/CMIP6Plus_CVs/actions/workflows/version_update.yml/badge.svg?branch=main'>
            </td>
        </tr>
        <tr>
            <td><strong>Repository Contents</strong></td>
<td><img src='https://img.shields.io/badge/Activities-%202%20-purple'>
<img src='https://img.shields.io/badge/Experiments-%2028%20-coral'>
<img src='https://img.shields.io/badge/Sources-%204%20-blue'></td></tr end>
        <tr>
            <td><strong>Interactions</strong></td>
            <td> <a href='https://github.com/WCRP-CMIP/CMIP6Plus_CVs/discussions'><img src='https://img.shields.io/github/discussions/WCRP-CMIP/CMIP6Plus_CVs?label=Discussions'></a>
            <a href='https://github.com/WCRP-CMIP/CMIP6Plus_CVs/issues'><img src='https://img.shields.io/github/issues/WCRP-CMIP/CMIP6Plus_CVs?label=Requests'></a>
            <img src="https://img.shields.io/github/contributors/WCRP-CMIP/CMIP6Plus_CVs">
           <img src='https://img.shields.io/github/commit-activity/m/WCRP-CMIP/CMIP6Plus_CVs?label=Commit%20Activity'>
           <img src='https://img.shields.io/github/last-commit/WCRP-CMIP/CMIP6Plus_CVs.svg'/> 
        </td>
        </tr>
    </table>
</div>

<br>


# 

## For information on how to interact
Visit the wiki using the button above, or [this link](https://github.com/WCRP-CMIP/CMIP6Plus_CVs/wiki)

## Currently active MIPs

To see a listing of currently active or planning activities/MIPs, please review details on the [Model Intercomparison Projects (MIPs)](https://wcrp-cmip.org/model-intercomparison-projects-mips/) page on the CMIP website.

## Registering Institutions, Models, or requesting changes to CVs:

To register your institution or model or to register a new activity/MIP or experiment, please submit an issue/ticket following the instructions on the [CMIP6Plus_CVs issue page](https://github.com/WCRP-CMIP/CMIP6Plus_CVs/issues/new). Follow the same procedure to request a change in any other CV.

## Automatic generation of CV files. 
With every update to this repository a new CV file is generated to reflect the changes. This can be found at `CVs/CMIP6PLUS_CV.json`. 

With every new release (see versioning description), a copy of the latest active `CMIP6PLUS_CV.json` will be archived in the CVs directory with the format: `CMIP6PLUS_CV_<tag_number>.json`.

## Publishing to ESGF

- In order to publish, you will need `v5.2.1` of the esg-publisher software or later.  `pip install esgcet`

- Add the following entries to your `esg.yaml` file.

```
user_project_config:
  cmip6plus:
    CONST_ATTR:
      project: CMIP6Plus
    pid_prefix: '21.14100'
cmip6_clone: cmip6plus
```
- When running the `esgpublish` CLI ensure you have the `--project cmip6plus` in the command line.

## Contributors

[![Contributors](https://contrib.rocks/image?repo=WCRP-CMIP/CMIP6Plus_CVs)](https://github.com/WCRP-CMIP/CMIP6Plus_CVs/graphs/contributors)

Thanks to our contributors!


## Acknowledgement

The repository content has been collected from many contributors representing the Coupled Model Intercomparison Project phase 6+ (CMIP6Plus), including those from climate modeling groups and model intercomparison projects (MIPs) worldwide. The structure of content and tools required to maintain it was developed by climate and computer scientists from the Coupled Model Intercomparison Project International Project Office ([CMIP-IPO](https://wcrp-cmip.org/cmip-governance/project-office/)), the Program for Climate Model Diagnosis and Intercomparison ([PCMDI](https://pcmdi.llnl.gov/)) at Lawrence Livermore National Laboratory ([LLNL](https://www.llnl.gov/)), and the [UK MetOffice](https://www.metoffice.gov.uk/), with assistance from colleagues at the UK Centre for Environmental Data Analysis ([CEDA](https://www.ceda.ac.uk/)), the Deutsches Klimarechenzentrum ([DKRZ](https://www.dkrz.de/en/)) in Germany and the members of the Infrastructure for the European Network for Earth System Modelling ([IS-ENES](https://is.enes.org/)) consortium.

This work is sponsored by the Regional and Global Model Analysis ([RGMA](https://climatemodeling.science.energy.gov/program/regional-global-model-analysis)) program of the Earth and Environmental Systems Sciences Division ([EESSD](https://science.osti.gov/ber/Research/eessd)) in the Office of Biological and Environmental Research ([BER](https://science.osti.gov/ber)) within the Department of Energy's ([DOE](https://www.energy.gov/)) Office of Science ([OS](https://science.osti.gov/)). The work at PCMDI is performed under the auspices of the U.S. Department of Energy by Lawrence Livermore National Laboratory under Contract DE-AC52-07NA27344.

<p>
    <img src="https://pcmdi.github.io/assets/CMIP/100px-CMIP_Logo_RGB_Positive-square-96dpi.png"
         width="65"
         style="margin-right: 30px"
         title="Couple Model Intercomparison Project International Project Office"
         alt="Couple Model Intercomparison Project International Project Office"
    >&nbsp;
    <img src="https://pcmdi.github.io/assets/PCMDI/100px-PCMDI-Logo-NoText-square-png8.png"
         width="65"
         style="margin-right: 30px"
         title="Program for Climate Model Diagnosis and Intercomparison"
         alt="Program for Climate Model Diagnosis and Intercomparison"
    >&nbsp;
    <img src="https://pcmdi.github.io/assets/DOE/480px-DOE_Seal_Color.png"
         width="65"
         style="margin-right: 30px"
         title="United States Department of Energy"
         alt="United States Department of Energy"
    >&nbsp;
    <img src="https://pcmdi.github.io/assets/LLNL/212px-LLNLiconPMS286-WHITEBACKGROUND.png"
         width="65"
         style="margin-right: 30px"
         title="Lawrence Livermore National Laboratory"
         alt="Lawrence Livermore National Laboratory"
    >&nbsp;
    <img src="https://pcmdi.github.io/assets/MetOffice/100px-Met_Office_LogoBLACK.png"
         width="65"
         style="margin-right: 30px"
         title="UK Met Office"
         alt="UK Met Office"
    >
</p>
