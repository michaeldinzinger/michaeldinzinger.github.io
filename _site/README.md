# michaeldinzinger.github.io

```
<xsd:element name="asset">
    <xsd:complexType>
        <xsd:sequence>
            <xsd:element name="loc" minOccurs="0" type="xsd:anyURI">
                <xsd:annotation>
                  <xsd:documentation>
                    A URL pointing to the URL of a web asset, usable and relevant
                    for the purposes of Text and Data Mining.

                    OPTIONAL: If this LOC element remains undefined, the remaining
                    elements refer to the asset that is identified by the URL of
                    the parent's LOC element.
                  </xsd:documentation>
                </xsd:annotation>
            </xsd:element>

            <xsd:element name="loc" type="xsd:anyURI">
                <xsd:annotation>
                  <xsd:documentation>
                    A URL pointing to the URL of a web asset, usable and relevant
                    for the purposes of Text and Data Mining.
                    
                    OPTIONAL: If this LOC element remains undefined, the remaining
                    elements refer to the asset that is identified by the URL of
                    the parent's LOC element.
                  </xsd:documentation>
                </xsd:annotation>
            </xsd:element>
        </xsd:sequence>
    </xsd:complexType>
</xsd:element>
```
