---
title: hn-target
weight: 1
draft: false
# bookFlatSection: false
bookToc: false
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---

# hn-target

{{< hint info >}}
We will try to keep the documentation up to date with each update of each script.!
{{< /hint >}}

## exports

For more information about how to use the exports, contact us on discord.

{{< tabs "hntarget-exports" >}}
    {{< tab "addPed" >}}
   
    exports['hn-target']:addPed('model', 'anim', coords)

    # Example
    exports['hn-target']:addPed('a_f_y_bevhills_04', 'anim', vector4(100.35, -1077.02, 28.21, 239.06)
    {{< /tab >}}
    {{< tab "addObject" >}}
    exports['hn-target']:addObject('model',coords)
    
    # Example
    exports['hn-target']:addObject('model',coords)
    {{< /tab >}}
    {{< tab "AddTargetPeds" >}}
    exports[''hn-target']:addTargetPeds(name , model, distance,  options, BlackList, WhiteList)

    
    ## Markdown content
    # Example 
    exports['hn-target']:AddTargetPeds('hn-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'hn-carinsurance:open',
                key = 'hn-carinsurance:open',
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
    exports[''hn-target']:AddTargetObjects(name , model, distance,  options, BlackList, WhiteList)
    
    # Example 
    exports['hn-target']:AddTargetObjects('hn-carinsurance',{'a_f_y_bevhills_04'}, 3.0,
        {

            {
                event = 'hn-carinsurance:open',
                key = 'hn-carinsurance:open',
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

{{< hint warning >}}
these exports can be updated. it's still a beta.
{{< /hint >}}
