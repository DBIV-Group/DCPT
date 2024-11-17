# DCPT : **Driver multi-modal dataset for L3 takeover scenario**

## Overview

This repository contains a comprehensive dataset of driver takeover responses in automated driving scenarios, including upper-body video,first-person view videos, eye-tracking and head motion data recordings. The dataset will be made public following the publication of our research paper.

## Dataset Structure

The repository is organized into four main folders:

- `Upper_body_video/`: Contains upper body video recordings of participants
- `First_person_view_video/`: Contains First-person view video recordings of participants

- `Eye_Tracking/`: Contains eye movement data
- `Head_motion/`: Contains Head motion data

### Root Directory Files

- `Takeover-Time.xlsx`: Records take-over times for each experimental trial
- `information.xlsx`: Contains demographic information of all participants

### Upper body video data

#### Naming Convention

Upper body video files follow the naming pattern:

`<NDRT>_P<Person>_<Take-over Moment>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Take-over Moment`: Six-digit timestamp (MM:SS:FF)
  - First 2 digits: Minutes
  - Middle 2 digits: Seconds
  - Last 2 digits: Frame number
- `Take-over Time`: Response time in 0.1s units

#### Description

Located in `Upper_body_video/` with two subfolders:

1. ```
   Upper_body_video_raw/
   ```

   - Full take-over experiment recordings
   - Resolution: 1920 x 1080 pixels
   - Unprocessed footage

2. ```
   Upper_body_video_processed/
   ```

   - 2-second clips before take-over moment
   - Resolution: 160 x 224 pixels
   - Processed according to our prediction model requirements

### First person view video data

#### Naming Convention

First person view video files follow the naming pattern:

`<NDRT>_P<Person>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Take-over Time`: Response time in 0.1s units

First person view videos are divided by Take-over Moment, takeover request occurred in the final segment of the video

#### Description

Located in `First_person_view_video/` with two subfolders:

1. ```
   First_person_view_video_raw/
   ```

   - Full take-over experiment recordings
   - Resolution: 1280 x 720 pixels
   - Unprocessed footage

2. ```
   Upper_body_video_processed/
   ```

   - 2-second clips before take-over moment
   - Resolution: 224 x 224 pixels
   - Processed according to our prediction model requirements

### Eye-tracking&head motion data

#### Naming Convention

Eye-tracking&head motion files follow the naming pattern:

`<NDRT>_P<Person>_<Take-over Time>`

Where:

- `NDRT`: Non-driving related task ID (refer to Table II in our research paper)
- `Person`: Participant ID
- `Take-over Time`: Response time in 0.1s units

The Take-over Moment is marked as 'w#' in the Event column

#### Description

Located in `Sequence/`:

- Format: Excel spreadsheets
- Collected by Tobii Pro Glasses 2


## Acknowledgments

We thank all participants who contributed to this dataset.
