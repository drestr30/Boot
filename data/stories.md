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
* affirm
 - utter_fiebre
* affirm
 - utter_high_priority

## fever medium priority
 - utter_fiebre
* deny
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

#### Q&A paths

<<<<<<< HEAD
=======
## intent fear
* fear 
 - utter_fear

>>>>>>> QA_branch
## question self-care
* question_care
  - utter_answer_care

## question hand wash
* question_hands
  - utter_answer_hands

<<<<<<< HEAD
=======
## question covid
* question_covid
  - utter_answer_covid

## question covid spread
* question_covid_spread
 - utter_covid_spread

## question covid sintoms
* question_covid_sintoms
 - utter_covid_sintoms

## question sintoms duration
* question_sintoms_duration
  -utter_sintoms_duration

## question mask
* question_mask
  - utter_answer_mask

## question pet
* question_pet
  - utter_answer_pet

## question pandemia
* question_pandemia
  - utter_answer_pandemia

## superficie 
* question_superfice
  -utter_answer_superfice

>>>>>>> QA_branch
## say goodbye path
* goodbye
  - utter_goodbye

## who is path
* who
  - utter_iamabot

## fallback
  - utter_unclear

