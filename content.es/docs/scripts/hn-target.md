---
title: hn-target
weight: 1
geekdocNav: true
geekdocAlign: left
geekdocAnchor: false
---

{{< hint type=note >}}
We will try to keep the documentation up to date with each update of each script.!
{{< /hint >}}

# exports

It is planned to give you the information through the following exports

{{< tabs "hntarget-exports" >}}
    {{< tab "addPed" >}}
    exports['Laz-target']:addPed('model', 'anim',coords)
    
    # Example
    exports['Laz-target']:addPed('a_f_y_bevhills_04', 'anim', vector4(100.35, -1077.02, 28.21, 239.06)
    {{< /tab >}}
    {{< tab "addObject" >}}
    exports['Laz-target']:addObject('model',coords)
    
    # Example
    exports['Laz-target']:addObject('model',coords)
    {{< /tab >}}
    {{< tab "AddTargetPeds" >}}
    exports[''Laz-target']:addTargetPeds(name , model, distance,  options, BlackList, WhiteList)

    # Example 
    exports['Laz-target']:AddTargetPeds('Laz-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'Laz-carinsurance:open',
                key = 'Laz-carinsurance:open',
                label = 'Open'
            }
        },
        false,
        {    coords = {
                pos = vector3(100.35, -1077.02, 29.21),
                radius = 2.0
            }
        }
    )
    {{< /tab >}}
    {{< tab "AddTargetObjects" >}}
    exports[''Laz-target']:AddTargetObjects(name , model, distance,  options, BlackList, WhiteList)
    
    # Example 
    exports['Laz-target']:AddTargetObjects('Laz-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'Laz-carinsurance:open',
                key = 'Laz-carinsurance:open',
                label = 'Open'
            }
        },
        false,
        {    coords = {
                pos = vector3(100.35, -1077.02, 29.21),
                radius = 2.0
            }
        }
    )
    {{< /tab >}}
{{< /tabs >}}


{{< hint type=warning >}}
these exports can be updated. it's still a beta.
{{< /hint >}}