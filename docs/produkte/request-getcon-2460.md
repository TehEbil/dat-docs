---
title: "Request getContractList"
topic_id: "2460"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfrage der Vorgangsübersicht > Request getContractList"
---

# Request getContractList

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
    <soapenv:Header/>
    <soapenv:Body>
        <veh:getContractList>
            <!--Optional:-->
            <request>
                <restriction>
                    <datEcode>011940020020010</datEcode>
                    <createDateFrom>2015-09-01</createDateFrom>
                    <createDateTo>2016-09-01</createDateTo>
                    <registrationNumber/>
                    <vin/>
                </restriction>
                <settings>
                    <!--Optional:-->
                    <numberOfContractsReturned>25</numberOfContractsReturned>
                    <offset>0</offset>
                    <returnLanguage>de</returnLanguage>
                    <sortingCriterions>
                        <!--Optional:-->
                        <createDateTo>
                            <!--Optional: desc / asc-->
                            <order>desc</order>
                            <!--Optional:-->
                            <priority>1</priority>
                        </createDateTo>
                    </sortingCriterions>
                </settings>
            </request>
        </veh:getContractList>
    </soapenv:Body>
</soapenv:Envelope>
```
