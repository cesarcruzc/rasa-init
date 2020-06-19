## happy_path
* greet
    - find_facility_types
* inform{"facility_type": "xubh-q36u"}    
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
* inform{"facility_id": 4245}
    - find_healthcare_address
    - utter_address
* thanks
    - utter_noworries

## happy_path_multi_requests
* greet
    - find_facility_types
* inform{"facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
* inform{"facility_id": "747604"}
    - find_healthcare_address
    - utter_address
* search_provider{"facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
* inform{"facility_id": 4245}   
    - find_healthcare_address
    - utter_address

## happy_path2
* search_provider{"location": "Austin", "facility_type": "xubh-q36u"}
    - facility_form
    - form{"name": "facility_form"}
    - form{"name": null}
* inform{"facility_id": "450871"}
    - find_healthcare_address
    - utter_address
* thanks
    - utter_noworries

## story_goodbye
* goodbye
    - utter_goodbye

## story_thankyou
* thanks
    - utter_noworries

## New Story

* greet
    - find_facility_types
* inform{"facility_type":"xubh-q36u"}
    - slot{"facility_type":"xubh-q36u"}
    - facility_form
    - form{"name":"facility_form"}
    - slot{"facility_type":"xubh-q36u"}
    - slot{"facility_type":"xubh-q36u"}
    - slot{"requested_slot":"location"}
* inform{"location":"San Francisco"}
    - slot{"location":"San Francisco"}
    - facility_form
    - slot{"location":"San Francisco"}
    - form{"name":null}
    - slot{"requested_slot":null}
* inform{"facility_id":"050076"}
    - slot{"facility_id":"050076"}
    - find_healthcare_address
    - slot{"facility_address":"2425 Geary Blvd, San Francisco, CA 94115"}
    - utter_address
* thanks
    - utter_noworries

## New Story

* greet
    - find_facility_types
* inform{"facility_type":"b27b-2uc7"}
    - slot{"facility_type":"b27b-2uc7"}
    - facility_form
    - form{"name":"facility_form"}
    - slot{"facility_type":"b27b-2uc7"}
    - slot{"facility_type":"b27b-2uc7"}
    - slot{"requested_slot":"location"}
* inform{"location":"Elizabeth"}
    - slot{"location":"Elizabeth"}
    - facility_form
    - slot{"location":"Elizabeth"}
    - form{"name":null}
    - slot{"requested_slot":null}
* inform{"facility_id":"315483"}
    - slot{"facility_id":"315483"}
    - find_healthcare_address
    - slot{"facility_address":"456 Rahway Avenue, Elizabeth, NJ 07202"}
    - utter_address
* thanks
    - utter_noworries

## New Story

* greet
    - find_facility_types
* inform{"facility_type":"b27b-2uc7"}
    - slot{"facility_type":"b27b-2uc7"}
    - facility_form
    - form{"name":"facility_form"}
    - slot{"facility_type":"b27b-2uc7"}
    - slot{"facility_type":"b27b-2uc7"}
    - slot{"requested_slot":"location"}
* inform{"location":"San Frascisco"}
    - slot{"location":"San Frascisco"}
    - facility_form
    - slot{"location":"San Frascisco"}
    - form{"name":null}
    - slot{"requested_slot":null}
* inform{"location":"San Francisco"}
    - slot{"location":"San Francisco"}
    - find_facility_types
* inform{"facility_type":"xubh-q36u"}
    - slot{"facility_type":"xubh-q36u"}
    - facility_form
    - form{"name":"facility_form"}
    - slot{"facility_type":"xubh-q36u"}
    - slot{"location":"San Francisco"}
    - slot{"facility_type":"xubh-q36u"}
    - form{"name":null}
    - slot{"requested_slot":null}
* inform{"facility_id":"050076"}
    - slot{"facility_id":"050076"}
    - find_healthcare_address
    - slot{"facility_address":"2425 Geary Blvd, San Francisco, CA 94115"}
    - utter_address
* thanks
    - utter_noworries
