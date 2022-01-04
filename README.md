# StartVM-automation
A small PowerShell script to use in a Runbook in Azure Automation for starting a VM.

A couple of things needs to be altered in this PowerShell-script before you actually run it:</p>

<ul><li>Set $SAMI to the object ID of your Managed Identity of your Automation Account. You can find that in the Automation Account side menu under 'Identity'</li><li>Set $automationAccount to the name of your Automation Account</li></ul>

When calling this Runbook you will have four parameters in total. You need to give values to three of them:</p>

<ul><li>resourceGroup - The name of the resource group where your VM resides</li><li>VMName - The name of your VM</li><li>method - 'SA' for System Assigned. This refers to the identity of your Automation Account.</li></ul>

