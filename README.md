# no-show-appointment-analysis

## Introduction

### Dataset Description 
The no show apointment is a record of 110,527 medical appointments scheduled in Brazil. The dataset focuses on the unique characteristics of each patient that scheduled appointment and whether they missed the appointment or they attended the scheduled appointment.  
    <hr> PatientId         - this is a unique identifier for each Patient 
    <hr> AppointmentID     - this is a unique identifier for each appointment schedule 
    <hr> Gender            - this column shows whether the patient is either a male or a female
    <hr> ScheduledDay      - this shows the day and time at which the appointment was made
    <hr> AppointmentDay    - this records the day for which the appointment was scheduled for 
    <hr> Age               - the age of the patient is recorded here
    <hr> Neighbourhood     - the area where the client resides is recorded here 
    <hr> Scholarship       - medical insurance status of the patient. 0 means the patient has no insurance 
    <hr> Hipertension      - this column shows whether the patient has hypertension or not 
    <hr> Diabetes          - this records whether the client has diabetes or not    
    <hr> Handcap           - this records any physical challenge of the patient 
    <hr> SMS_received      - this records whether a reminder was sent to the patient or not
    <hr> No-show           - this column records whether the patient missed the appointment or not. No shows that the appointment was not missed. Yes means the appointment was missed. 
The dataset contains 110,527 rows of data with 14 columns. No row has missing data. A closer look shows that the ScheduleDay and AppointmentDay columns contain a mixture of date and time. And both columns are set as string. The Age column also has a '-1' as the age of a patient. 
To clean the ScheduleDay column will be split into two columns - schedule_day and schedule_time. Both of which will be set to the date time format.
The AppointmentDay columns as well contains date and time, however, the time is set to 00:00:00 for all the data. Thereby showing that the schedule time were not recorded. As such the time will be dropped and only the date kept.

### Question(s) for Analysis
<hr> What proportion of appointments get missed?
<hr> Is gender a predictor of missing appointment? if yes, by what proportion?
<hr> Is age a predictor of missing appointments?
<hr> Do underlying health conditions predict missing appointments?


## Conclusions
### Results show that 
<hr> About 20.2% of all appointments scheduled are missed by patients.
<hr> About 19.96% of Men missed scheduled appointments while about 20.31% of women missed scheduled appointments. More women
  tend to miss their appointments but the margin is close as not to be a reliable predictor of missing appointment
<hr> youth missed the highest proportion of appointment scheduled, followed by mature I, then Children, mature II. Infants missed about 18% of their scheduled appointments followed by the senile, pre_senile, mature III and long lifers missed the lowest percentage of appointments.
<hr> Patients with no healthy challenge such as diabetes tend to miss more appointments as about 20.92% of them missed their scheduled appointments while only 17.86% of people with health challenges missed their scheduled appointments. 

### Limitation of the data exploration
<hr> This analysis did not carry out any hypothesis testing. As such it is impossible to claim that the difference recorded in the results are statistically significant 
        
