# DCPT : **A Multi-Modal Dataset of Drivers' Cognitive and Physical States in L3 Takeover Scenarios**

## Overview

This repository contains a specialized dataset of driver takeover responses in automated driving scenarios, including upper-body video,first-person view videos, eye-tracking and head motion data recordings. The dataset will be made public following the publication of our research paper.

## Dataset Samples
You can download the processed dataset from [Google Drive](https://drive.google.com/drive/folders/1lDjkdJyDSnzDA995m1h4Mi-j74Ipi91_?usp=drive_link). If you need the raw files, please contact me at liangyh23@mails.jlu.edu.cn.

## Dataset Structure

The repository is organized into four main folders:

- `Upper_body_video/`: Contains upper body video recordings of participants
- `First_person_view_video/`: Contains First-person view video recordings of participants
- `Eye-tracking&head motion data/`: Contains eye movement&head motion data


### Root Directory Files

- `Takeover-Time.xlsx`: Records take-over times for each experimental trial
- `information.xlsx`: Contains demographic information of all participants

### Upper body video data

#### Naming Convention

Upper body video files follow the naming pattern:

`<NDRT>_P<Person>_<Date>_<Hour>_<Minute>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Date`: Recording date in YYYYMMDD format
- `Hour`: Recording start hour in HH format
- `Minute`: Recording start minute in MM format
- `Take-over Time`: Response time in 0.1s units

#### Description

- 2-second clips before the take-over request was issued
- Resolution: 160 x 224 pixels
- Processed according to our prediction model requirements

### First person view video data

#### Naming Convention

First person view video files follow the naming pattern:

`<NDRT>_P<Person>_<Date>_<Hour>_<Minute>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Date`: Recording date in YYYYMMDD format
- `Hour`: Recording start hour in HH format
- `Minute`: Recording start minute in MM format
- `Take-over Time`: Response time in 0.1s units

#### Description

- 2-second clips before the take-over request was issued
- Resolution: 224 x 224 pixels
- Processed according to our prediction model requirements

### Eye-tracking&head motion data

#### Naming Convention

Eye-tracking&head motion files follow the naming pattern:

`<NDRT>_P<Person>_<Date>_<Hour>_<Minute>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Date`: Recording date in YYYYMMDD format
- `Hour`: Recording start hour in HH format
- `Minute`: Recording start minute in MM format
- `Take-over Time`: Response time in 0.1s units

The moment when the take-over request is issued is marked as 'w#' in the Event column.

#### Description

- Format: Excel spreadsheets
- Collected by Tobii Pro Glasses 2


## Acknowledgments

We thank all participants who contributed to this dataset.
