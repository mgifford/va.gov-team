# Text messages and Error Messages 
This document will serve as hub to all the source of truths documentation for all check-in and pre-check-in text message and error message wording.

Jump to...
- [Check-in](#checkin)
- [Pre-check-in](#precheckin)

## Check-in <a name="checkin"></a> 
This [Sketch file](https://www.sketch.com/s/e79a827e-42cf-4a82-b554-874c75b5c70e/a/3Op54Vm) shows the overall user flow and decision points. However, the Sketch document is not the source of truth. It will be updated periodically, but may be out-of-date.

### VeText 

VeText's [source of truth](https://github.com/department-of-veterans-affairs/vetext-docs/blob/master/README.md). (As of Feb. 3, 2022, VeText is still working through their documentation on the linked page, but the above Sketch file includes VeText messaging.)

### CHIP

CHIP's [source of truth](https://github.com/department-of-veterans-affairs/chip/blob/master/docs/chip-messaging.md).

### VA.gov

| Scenario | Message | Visual (will update to Sketch link) |
| --- | --- | --- |
| Identity Verification: last name and last 4 SSN do not match record AND the Veteran has attempted verification 2 or less times. (this will stay on the auth page and  lastName and lastFour prompts remain on screen) | We're sorry. We couldn't match your information to our records. Please try again. | <img width="250" alt="less than 3 retries" src="https://user-images.githubusercontent.com/90633685/159027360-6a543295-79ad-4ea0-85f2-69e2fc681a4b.png"> [sketch link](https://www.sketch.com/s/e79a827e-42cf-4a82-b554-874c75b5c70e/a/1KMbqy4)|
| Identity Verification: last name and last 4 SSN do not match record AND the Veteran has attempted verification 3 or more than 3 times. (this will load the error page without lastName and lastFour prompts | (header) We couldn't check you in (body) We’re sorry. We couldn't match your information to our records. Please ask a staff member for help. |   <img width="253" alt="ci-more than 3 retries" src="https://user-images.githubusercontent.com/90633685/158430062-ca29bef2-c614-431c-b8e2-bb9ce9ffd99a.png"> [sketch link](https://www.sketch.com/s/e79a827e-42cf-4a82-b554-874c75b5c70e/a/ZOo3YgY)
| Is the system operational? (Any bad request from the server)| (header) We couldn't check you in (body) We're sorry. Something went wrong on our end. Check in with a staff member. | ![generic error](https://user-images.githubusercontent.com/66287082/152366754-44736746-4e6e-4753-9a3a-7c17c5383844.png) |
| This error shows when Spanish/Tagalog-speaking user chooses to see the check-in content in preferred language, but there is some English content on the page.| Some content may be in English. (Alert will be displayed in the choosen laguage.)|  ![image](https://user-images.githubusercontent.com/91493630/170539202-1810d2a3-07a5-4f2a-a8f0-77f9acc020fa.png)   [Wireframe-1](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/ag2OVVz)  [Wireframe-2](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/DPOR88y) |

## Pre-check-in <a name="precheckin"></a> 
The follwing Sketch files (linkes below) show the overall user flow and decision points for both Read-only and Editing versions. However, the Sketch document is not the source of truth. It will be updated periodically, but may be out-of-date.
  - [Read-only verion](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/qeOEgjk)
  - [Editing verion](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/Gm7yvkE)

| Scenario | Message | Visual (will update to Sketch link) |
| --- | --- | --- |
| Identity Verification: last name and DOB do not match record AND the Veteran has attempted verification 2 or less times | We're sorry. We couldn't match your information to our records. Please try again. | <img width="250" alt="less than 3 retries" src="https://user-images.githubusercontent.com/90633685/159027360-6a543295-79ad-4ea0-85f2-69e2fc681a4b.png"> [sketch link](https://www.sketch.com/s/e79a827e-42cf-4a82-b554-874c75b5c70e/a/Qb5E7q7)|
| Identity Verification: last name and last 4 SSN do not match record AND the Veteran has attempted verification 3 or more than 3 times. (this will load the error page without lastName and lastFour prompts | We're sorry. We couldn't match your information to our records. Please call us at 800-698-2411 (TTY:711) for help signing in. |<img width="284" alt="pci-more than 3 retries" src="https://user-images.githubusercontent.com/90633685/159040004-5ce9c48a-d6e4-4dab-9f9e-1676a77f41f8.png"> [sketch link](https://www.sketch.com/s/e79a827e-42cf-4a82-b554-874c75b5c70e/a/JndY4v0) |
| Link expired (No UUID) | (header) Sorry, we can't complete pre-check-in (body) You can still check-in with your phone once you arrive at your appointment. | <img width="240" alt="Link expired (no UUID)" src="https://user-images.githubusercontent.com/91493630/187524442-e00d7547-38e3-41ab-bd0d-fdf63615f7f6.png"> sketch (tbd) |
| Is the system operational? (Any bad request from the server) | (header) We couldn't check you in (body) We're sorry. Something went wrong on our end. Check in with a staff member. | ![generic error](https://user-images.githubusercontent.com/66287082/152366754-44736746-4e6e-4753-9a3a-7c17c5383844.png) |
| User accidentally goes back / navigates out of the editing mode. Or user cancels out of the editing mode| (header) Are you sure? (body) You haven’t finished editing your <auto-generated>. If you cancel, your in-progress work won’t be saved.| ![back navigation/edit cancel](https://user-images.githubusercontent.com/91493630/156664030-c0833109-fe0a-4cda-952d-ac96e4f6a51b.png) [Wireframe](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/v/15dwW8/a/4an9O8A/r/lOabWV#Inspector) |
| This error shows when Spanish/Tagalog-speaking user chooses to see the pre-check-in content in preferred language, but there is some English content on the page.| Some content may be in English. (Alert will be displayed in the choosen laguage.)|  ![image](https://user-images.githubusercontent.com/91493630/170539202-1810d2a3-07a5-4f2a-a8f0-77f9acc020fa.png)   [Wireframe-1](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/ag2OVVz)  [Wireframe-2](https://www.sketch.com/s/5331b114-280d-4ff5-8d36-ec49b1696b9e/a/DPOR88y) |
  
  
  


  





  
  



