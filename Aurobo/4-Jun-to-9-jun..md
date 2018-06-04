# Sprint Planning (04-Jun-2017 to 09-Jun-2018)

## Abstract goal

* In next sprint we should be able to fialize the data by which we will be releasing the application and put a Demo on Aurobo.in. So in the current sptint we are thinking that, we should have all unknown part of clear and also figure out if there is something we can automate or remove hurdles in the development if any

## Current sprint tasks:

### Packages

* The packaging found to be one the major issue to reuse the code. We decided to have 3 packages **Plasma**, **Anatomy** and **UI-components**

#### Considerations about packages:

* All the packages would be in local for now so that won't have to worry about their version while in development
* They should be in ready to publish state by end of sprint
* Anatomy will be dependent on the Plasma, but that will be fine for our need

### Creat & Update -> SET

* During the sprint planning we suddenly went to the discussion about the task of Plasma.Update feature. And then thought, how about to have single feature for CREATE and UPDATE, i.e. SET . It seems sensible as Ronak said if take phylosophy of the firebase
* We have many discussions on
* * how to handle different cases where CREATE and UPDATE both works differently
* * How to handle different batch operations because we want to conver many UI cases by which the user of the lbrary may want to utilize like 1) while creating salesOrder and salesOrderItems both will be passed, 2)with update user may want to save individual entities and many others

### UI Component

* They will be extended segmentic UI. We will currently focus on Quantity, Date, Dropdown, FileInput controls
