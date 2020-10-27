Scheduled VM Resizes with Resource Groups
=========================================

            

Through this Automation script you can schedule a specific Resource Group Azure VM at specific times for resizing. By resizing Resource Group VMs during low traffic hours, the computational costs are reduced.


Check the  step-by-step deployment guide on GitHub here [https://siebertt.github.io/Azure-ResourcegroupVM-Rescaling-Scheduler/](https://siebertt.github.io/Azure-ResourcegroupVM-Rescaling-Scheduler/)


It is suggested that you run 2 schedules, for example:


  *  At night hours, downscale to the lowest possible VM size to reduce the related costs.

  *  At the start of office hours, upscale to the usual size for productivity. 

This script is highly based on Kay Singh's script for Vertical Scaling, I added scheduling variables for practical use.


Check his Runbook here: [https://docs.microsoft.com/en-us/azure/virtual-machines/virtual-machines-linux-vertical-scaling-automation](https://docs.microsoft.com/en-us/azure/virtual-machines/virtual-machines-linux-vertical-scaling-automation)


*Notes: Downtime of +- 4 minutes applies when the job starts. Take this into account when applying this Runbook to production VMs.*


*You can only resize to VM Sizes that have the same number of disks or more. Check the VM Sizes list on Technet for more information.*


*This Runbook does not work for Classic VMs.*


 


 


 


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
