## greet path
* greet
  - utter_greet
* affirm OR sick
  - utter_question_sintoms

## sick path contact high priority
* sintoms_priority
  - utter_fiebre
* affirm
  - utter_covid_contact
* affirm
  - utter_high_priority

## sick path country priority
* sintoms_priority
  - utter_fiebre
* affirm
  - utter_covid_contact
* deny 
  - utter_country_contact
* affirm
  - utter_high_priority

## sick path contact mild priority
* sintoms_priority
  - utter_fiebre
* deny
  - utter_covid_contact
* affirm 
  - utter_mild_priority

## sick path country mild priority
* sintoms_priority
  - utter_fiebre
* deny
  - utter_covid_contact
* deny 
  - utter_country_contact
* affirm
  - utter_mild_priority 

## sick path no contact mild priority
* sintoms_priority
  - utter_fiebre
* affirm
  - utter_covid_contact
* deny 
  - utter_country_contact
* deny
  - utter_mild_priority

## sick path no contact mild priority
* sintoms_priority
  - utter_fiebre
* deny
  - utter_covid_contact
* deny 
  - utter_country_contact
* deny
  - utter_not_emergency

######

## soft sintoms path
* sintoms_mild 
 - utter_covid_contact

## no contact path
* sintoms_mild 
  - utter_covid_contact
* deny
  - utter_country_contact
* deny
  - utter_fiebre
* deny
  - utter_not_emergency

## no contact no fiber
* sintoms_negative
  - utter_covid_contact
* deny
  - utter_country_contact
* deny
  - utter_not_emergency

## Covid contact positive fiebre
* sintoms_mild OR sintoms_negative
  - utter_covid_contact
* affirm
  - utter_fiebre
* affirm
  - utter_high_priority

## country contact positive
* sintoms_mild OR sintoms_negative
 - utter_covid_contact
* deny
 - utter_country_contact
*affirm
 - utter_fiebre
* affirm
 - utter_high_priority

## fever medium priority
 - utter_fiebre
*deny
 - utter_mild_priority

## sick path negative
* greet
  - utter_greet
* sick
  - utter_question_sintoms
* sintoms_negative
  - utter_covid_contact
* deny
  - utter_country_contact
* deny
  - utter_not_emergency

## say goodbye path
* goodbye
  - utter_goodbye

## who is path
* who
  - utter_iamabot

## fallback
  - utter_unclear

