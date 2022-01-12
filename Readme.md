
#########################
##  Ashnik Assignment  ##
#########################

Task
####
Refer assignement.md

Solution
########

Use the below link to create a PVC 

https://aws.amazon.com/blogs/containers/introducing-efs-csi-dynamic-provisioning/

Use the below command to deploy helm chart assuming you have Ingress, metric server in place.

helm install wiki ./wiki-0.0.2.tgz -n wiki --set persistence.enabled=true --set persistence.existingClaim=efs-claim --debug 

Output of the --dry-run is added as output.txt

Note: -

    To accomadate the persistent volume go code was added with a storage path.