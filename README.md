# Ders12ekim2018
<?xml version="1.0"?>
<flowgorithm fileversion="2.6">
    <attributes>
        <attribute name="name" value=""/>
        <attribute name="authors" value="12"/>
        <attribute name="about" value=""/>
        <attribute name="saved" value="2018-10-12 10:56:00 "/>
        <attribute name="created" value="MTI7IFBDMTI7IDIwMTgtMTAtMTI7IDEwOjQ3OjE4IDsgMTU2NA=="/>
        <attribute name="edited" value="MTI7IFBDMTI7IDIwMTgtMTAtMTI7IDEwOjU2OjAwIDsgMTU1NQ=="/>
    </attributes>
    <function name="Main" type="None" variable="">
        <parameters/>
        <body>
            <declare name="saat, dakika, saatekle, saataci" type="Real" array="False" size=""/>
            <declare name="aci" type="Real" array="False" size=""/>
            <output expression="&quot;SAAT&#304; G&#304;R&#304;N&#304;Z&quot;"/>
            <input variable="saat"/>
            <output expression="&quot;DAK&#304;KAYI G&#304;R&#304;N&#304;Z&quot;"/>
            <input variable="dakika"/>
            <assign variable="saataci" expression="((dakika/2)+(saat*30))-(dakika*6)"/>
            <if expression="saataci&lt;0">
                <then>
                    <assign variable="saataci" expression="saataci*-1"/>
                </then>
                <else/>
            </if>
            <output expression="saataci"/>
        </body>
    </function>
</flowgorithm>
