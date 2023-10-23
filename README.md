# bmi-calculator-api
SOAP web service allows to calculate BMI (Body Mass Index) based on weight and height, and provide a category according to WHO.

## Request:
POST /calculator 

HTTP/1.1

Host: 0.0.0.0:8081

Content-Type: text/xml;charset=UTF-8

soapaction: http://mulesoft.org/calculator/CalculateAdultBMI

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:bmi="http://mulesoft.org/calculator">
   <soapenv:Header/>
   <soapenv:Body>
      <bmi:CalculateAdultBMIRequest>
         <weight>?</weight>
         <height>?</height>
      </bmi:CalculateAdultBMIRequest>
   </soapenv:Body>
</soapenv:Envelope>
```
