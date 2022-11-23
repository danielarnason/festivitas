# Festivitas modul
Et modul til at give lidt ekstra festivitasstemning til Spatial Suite.

## Installation


1. **Tilføj modul til den ønskede modulfil**  
`<module dir="custom/festivitas" name="festivitas" permissionlevel="public"/>`

2. **Editer parametrene i deploy filen, så det hele virker hos dig!**  
Parameteren _festivitas.skin\_name_ skal indeholde navnet på det skin, som bliver brugt. Her i Slagelse hedder det skin vi bruger _base\_custom_, så parameteren ser sådan her ud;  
`<param name"festivitas.skin_name">base_custom</param>`  
Parameteren _festivitas.ventetid_ angiver hvor lang tid i millisekunder, der skal gå, indtil julemanden, rensdyret og pingvinen begynder at kigge frem. Her i Slagelse skal der gå 5 minutter inden de kigger frem, så parameteren ser sådan her ud;  
`<param name="festivitas.ventetid">300000</param>`  
Konverter fra minutter til millisekunder sådan her: Minutter * 60 * 1000 :)

3. **Tilføj tool til den relevante profil.**  
For en julemandsknap;  
`<tool module="festivitas" name="festivitas"/>`  
For en skjult julesurprise, der begynder efter lidt tid;  
`<tool module="festivitas" name="festivitas_plugin"/>` 
