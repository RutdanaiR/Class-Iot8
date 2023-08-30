## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301028/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301028/model-01/sn-001
    - payload
        - {"temperature": "25"}
        - {"weight_cloth": "3"}
        - {"inbalance": "9"}
        - {"rotation": "20"}
        - {"้huminity": "50"}
        - {"load": "5"}
        - {"water_level": "4"}
        - {"detergent": "2"}
        - {"noise_anomaly": "2"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301028/model-01/sn-001
    - payload
        - {"temperature": "40"}
        - {"huminity": "30"}
        - {"vibration": "0.5"}
        - {"radar": "1"}
        - {"current": "100"}
        - {"air_pressure": "200"}
        - {"touch_open/close": "0"}