---
title: "hn-logs"
weight: 2
draft: false
# bookFlatSection: false
# bookToc: true
# bookHidden: false
# bookCollapseSection: false
# bookComments: false
# bookSearchExclude: false
---
# hn-logs

Standalone system to create logs on our server

## hn-logs:LogFields
{{< tabs "hnlogs-logfields" >}}
    {{< tab "client" >}}
    TriggerServerEvent('hn-Logs:LogFields',
        typewebhook,
        title,
        Description,
        color,
        footer,
        field,
        id,
        tag -- true or false
    )
    {{< /tab >}}
    {{< tab "server" >}}
    TriggerEvent('hn-Logs:LogFields',
        typewebhook,
        title,
        Description,
        color,
        footer,
        field,
        id,
        tag  -- true or false
    )
    {{< /tab >}}
{{< /tabs >}}

### field

{{< hint >}}
    field = {
        name = 'option Title',
        value = 'option value',
        inline = true --true or false
    }
{{< /hint >}}

{{< hint warning >}}
    ### Disable description
    TriggerServerEvent('hn-Logs:LogFields',
        typewebhook,
        title,
        false,
        color,
        footer,
        field,
        id,
        tag -- true pr false
    )
{{< /hint >}}
{{< hint info >}}
    ### Enable Mentions
    TriggerServerEvent('hn-Logs:LogFields',
        typewebhook,
        title,
        description,
        color,
        footer,
        field,
        id,
        true
    )
{{< /hint >}}


## hn-logs:SimplyLog
{{< tabs "hnlogs-simplylogs" >}}
    {{< tab "client" >}}
    TriggerServerEvent('hn-Logs:SimplyLog',
        typewebhook,
        title,
        color,
        'Inventario',
        text,
        tag -- true or false
    )
    {{< /tab >}}
    {{< tab "server" >}}
    TriggerEvent('hn-Logs:SimplyLog',
        typewebhook,
        title,
        color,
        'Inventario',
        text,
        tag -- true or false
    )
    {{< /tab >}}
{{< /tabs >}}
