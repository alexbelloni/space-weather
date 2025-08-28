SPACE WEATHER

Space weather is the dynamic set of conditions in the space environment surrounding Earth, shaped largely by the Sun’s energetic emissions and magnetic activity. Unlike terrestrial weather, driven by temperature, humidity, and air pressure, space weather encompasses solar wind, solar flares, coronal mass ejections, and variations in the solar magnetic field that travel outward through the solar system, often impacting Earth’s magnetic field and atmosphere.

These solar phenomena can disrupt satellite operations, interfere with communication and navigation systems, threaten astronaut safety, and even affect terrestrial power grids. Though the Sun sits 150 million kilometers away, its constant output of energy affects Earth’s environment and modern technology. Understanding and forecasting space weather is critical for protecting infrastructure and daily life in an increasingly interconnected and space-reliant world.

Bringing the space weather subject to our table, there are many APIS or datasets related to it on the intenet. The NOAA Space Weather Prediction Center (SWPC) provides a dedicated system of Alerts, Watches, and Warnings for space weather, which inform the public and stakeholders about expected solar activity levels and their possible impacts on Earth’s environment, for instance.

On this project, I test some resource related to the space weather.  

Events by NOAA (edited_events.json)
https://services.swpc.noaa.gov/json

|Attribute |Meaning |
|--------------|--------------------------------------------------------------------------------------------------------|
|begin_datetime|Date and time the event began (UTC, ISO 8601 standard). |
|begin_quality |Quality of the beginning record, usually indicating reliability (when filled in). |
|max_datetime |Date/time the event reached maximum intensity. |
|max_quality |Quality of the record of the maximum of the event. |
|end_datetime |Date/time the event ended. |
|end_quality |Quality of the end record. |
|observatory |Code of the observatory that recorded the event (“G19” probably indicates GOES-19). |
|quality |Degree of reliability or quality of the event, scale 0-5 (the higher the better). Minor, Moderate, Strong, Severe, Extreme |
|type |Type of event (“XRA” stands for Solar X-Ray, typical of solar flares). XRA,FLA,RSP,RBR,BSL,DSF,EPL,LPS,RNS | |coded_type |Numeric code representing the type of event. |
|obsid |Event identifier for a specific observatory/system. |
|location |Location of the event on the Sun (may be empty if not identified). |
|frequency |Observed frequency range, in this case 1-8 Ångströms (“1-8A”), typical for X-ray flares. |
|particulars1 |Event class (e.g., “C5.4,” indicating a class C flare with an intensity of 5.4). |
|particulars2 |Maximum observed flux, typically in Watts/m² (e.g., “3.7E-03”). |
|particulars3–9 |Extra details, such as fluxes at frequencies, durations, or other specific values; may be null if not applicable. |
|particulars10 |Other specific data, often related to decay or other additional reading. | |region |Solar active region associated with the event (may be null if undefined). |
|bin |Internal or grouping identifier for data processing. |
|age |Event status (“new” indicates a recently detected event). |
|status_code |Status code (e.g., “2” may indicate active/registered). |
|status_text |Free text about the status (here, “-” indicates no additional information). |
|change_flag |Indicates whether there has been a recent change in the event data (1 = yes). |


Flares and Eruptions  
XRA: A general X-ray event detected by the GOES satellite system. The X-ray flux is a key indicator of solar flare intensity, and events above a certain threshold (M5) can trigger a radio blackout alert.  
FLA: An optical flare observed in the hydrogen-alpha (H-alpha) wavelength. H-alpha is a specific reddish visible light emitted by hydrogen, and these flares are classified by their area and brightness.  
BSL: Bright Surge on the Limb. This is a bright, transient solar feature seen at the edge (or limb) of the Sun.  
DSF: Filament Disappearance. This occurs when a solar filament—a large, cool, and dense cloud of plasma suspended above the Sun's surface by magnetic forces—erupts or dissipates.  
EPL: Eruptive Prominence on the Limb. This is a large, often spectacular, solar prominence that erupts from the Sun's edge into space.  
LPS: Loop Prominence System. A system of loop-like plasma structures, often formed after a solar flare.    
Radio Bursts  
RSP: Sweep-frequency radio burst. A type of radio emission from the Sun that "sweeps" through a range of frequencies over time. These bursts are classified into types (e.g., Type II, III, IV) based on their characteristics.  
RBR: Fixed-frequency radio burst. A radio burst detected at a single, fixed frequency. NOAA monitors these bursts at several standard frequencies.  
RNS: Radio Noise Storm. A prolonged, high-intensity radio emission from the Sun, typically at meter wavelengths. 

https://www.swpc.noaa.gov/sites/default/files/images/FINAL%20SWPC%20User%20Needs%20Report-1.pdf

Observatory  

G18 and G19 refers to the GOES-18 and GOES-19, advanced environmental satellites  
HOL	Holloman Air Force Base, New Mexico, USA	One of the SOON network observatories that records and reports solar activity.  
PAL	Palahua, Hawaii, USA	A SOON network observatory that has been used to report on solar flares and radio bursts.  
SAG	Sagamore Hill, Massachusetts, USA	A SOON network observatory that reports on solar radio bursts.  
SVI	San Vito, Italy	A SOON network observatory that reports on solar radio bursts.  
LEA	Learmonth, Australia	One of the SOON observatories operated by the U.S. Air Force to monitor solar activity.

