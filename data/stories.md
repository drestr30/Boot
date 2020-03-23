## greet path
* greet
  - utter_greet
* affirm
  - utter_question_sintoms

## sick path high priority
* greet
  - utter_greet
* sick

## high priority
  - utter_question_sintoms
* sintoms_priority
  - utter_high_priority

## mild priority
 - utter_question_sintoms
*sintoms_mild
  - utter_covid_contact

## low priority 
  - utter_question_sintoms
*sintoms_negative
  - utter_covid_contact

## Covid contact positive
  - utter_covid_contact
*affirm
  - utter_fiebre

## Covid contact negative
  - utter_covid_contact
*deny
 - utter_country_contact

## country contact positive
 - utter_country_contact
*affirm
 - utter_fiebre

## country contact negative
 - utter_country_contact
*deny
 - utter_not_emergency

## fever high priority
 - utter_fiebre
*affirm
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
  -utter_covid_contact
* deny
  -utter_country_contact
* deny
 -utter_fiebre
* deny
  - utter_not_emergency

## say goodbye path
* goodbye
  - utter_goodbye

## who is path
* who
  -utter_iamabot

