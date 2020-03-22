## sick path high priority
* greet
  - utter_greet
* sick
  - utter_question_sintoms
* sintoms_priority
  - utter_high_priority

## covid contact mild
*sintoms_mild
  - utter_covid_contact
*affirm
  - utter_fiebre
*deny
  - utter_mild_priority

## country contact mild
 - utter_covid_contact
*deny
 - utter_country_contact
*affirm
- utter_fiebre
*deny
 - utter_mild_priority

## fever high priority
 - utter_fiebre
*affirm
 - utter_high_priority


## country contact positive
*sintoms_negative
  - utter_country_contact
*affirm
  - utter_fiebre
*affirm
  -utter_high_priority

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
  - utter_not_emergency

## say goodbye path
* goodbye
  - utter_goodbye

## who is path
* who
  -utter_iamabot
