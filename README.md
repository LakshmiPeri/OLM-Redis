# Installing Redis Enterprise Operator on Openshift's OLM
## Overview
One way to install Redis Enterprise Operator is using Openshift's marketplace for operators - OLM.
This is a quick steps to achieve that. 
  1. Apply scc.yaml. 
  2. Install the OLM operator. 
  3. Deploy rec cluster. 
  4. Deploy rec database. 

### Pre-requisites. 
 Create a new project in Openshift. 
   * oc new-project demo-olm
   * oc apply -f openshift/scc.yaml. **This needs to be modified if you intent to have a seperate name of cluster than rec**. 
 
 Install Redis enterprise operator from Operator hub 
 ![image](https://user-images.githubusercontent.com/84194562/157730404-01dbcede-91ee-4fa2-a45d-6c29a1d6698e.png)

