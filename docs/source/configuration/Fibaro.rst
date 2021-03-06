Fibaro 
======================

.. _fibaro_door_window_sensor:

Door and Window Sensor    
----------------------


.. image:: ../_static/images/fibaro_door_window_sensor.jpg 
   :align: center


Wake-up device 
~~~~~~~~~~~~~~~
This device is waken by opening/closing  


Configuration   
~~~~~~~~~~~~~~~~

The Door and Window Sensor can send a dimmer value to the associated devices when it is open. And the dimmer value is either from 1 to 99 or 255.  

.. list-table::  
   :widths: 15 30
   :header-rows: 1

   * - Signal Trigger Device 
     - Description    
   * - 1 to 99 or 255   
     - 1 to 99: Send dimming level to associated dimmers. 255: Send ON command to associated devices   


.. _fibaro_config_flood_sensor:

Flood sensor     
----------------------


.. image:: ../_static/images/fibaro_flood_sensor.jpg 
   :align: center



Wake-up device 
~~~~~~~~~~~~~~~
This device is waken by opening/closing


Configuration   
~~~~~~~~~~~~~~~~ 

The following configuration determines a type of command frame sent by the Sensor in case flooding has been detected or cancelled.

.. list-table::  
   :widths: 15 30
   :header-rows: 1

   * - Alarm Type
     - Description    
   * - Alarm Water   
     - Send an ALARM when the flooding has been detected   
   * - BASIC SET 
     - The associated devices are triggered ON when the flooding has been detected  



Changes of visual and acoustic affect allow to increase the battery life. This can be configured as follows 

.. list-table::  
   :widths: 15 30
   :header-rows: 1

   * - Visual and Acoustic Affect
     - Description    
   * - Nothing     
     - Deactivate visual and acoustic affect     
   * - Visual affect
     - Activate the visual effect     
   * - Acoustic affect 
     - Activate the acoustic affect  
   * - Acoustic and Visual affect
     - Activate both visual and acoustic affect  



The parameter allows for LED indicator and acoustic alarm deactivation in case of flooding detection


.. The following configuration determines if an alarm is sent to the devices when either tamper or flooding happens.  

.. .. list-table::  
..    :widths: 15 30
..    :header-rows: 1

..    * - Signal Trigger Device 
..      - Description    
..    * - Nothing     
..      - Do not send nether tamper nor flooding event     
..    * - Flooding    
..      - Send flooding event    
..    * - Tamper 
..      - Send tamper event 
..    * - Flooding, tamper 
..      - Send flooding and tamper event 


When the flooding event is triggered, it will send a Flood Alarm.
When the flooding event is ceased, it will send another Flood Alarm which cancels the flooding event. 
The following configuration is to configure a time period that the Flood Alarm is sent since the flooding event is ceased. 

.. list-table::  
   :widths: 15 30
   :header-rows: 1

   * - Interval Time
     - Description    
   * - 0 to 3600
     - A period that the Flood Alarm is sent since the flooding event is ceased. 


.. _fibaro_config_motion_detector_sensor:

Motion sensor     
----------------------


.. image:: ../_static/images/fibaro_motion_sensor.png 
   :align: center


Wake-up device 
~~~~~~~~~~~~~~~
This device is waken by making a motion in front of the device


Configuration   
~~~~~~~~~~~~~~~~ 

When the motion event is triggered, it will send a Motion Alarm.
When the motion event is ceased, it will send another Motion Alarm which cancels the motion event. 
The following configuration is to configure a time period that the Motion Alarm is sent since the motion event is ceased. 

.. list-table::  
   :widths: 15 30
   :header-rows: 1

   * - Interval Time
     - Description    
   * - 1 to 65535
     - A period that the Motion Alarm is sent since the motion event is ceased. 


.. An example of configuration    
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 

