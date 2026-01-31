```
> operator-sdk olm install
INFO[0000] Fetching CRDs for version "0.28.0"
INFO[0000] Fetching resources for resolved version "v0.28.0"
INFO[0002] Checking for existing OLM CRDs
INFO[0002] Checking for existing OLM resources
INFO[0002] Installing OLM CRDs...
INFO[0002]   Creating CustomResourceDefinition "catalogsources.operators.coreos.com"
INFO[0003]   CustomResourceDefinition "catalogsources.operators.coreos.com" created
INFO[0003]   Creating CustomResourceDefinition "clusterserviceversions.operators.coreos.com"
INFO[0004]   CustomResourceDefinition "clusterserviceversions.operators.coreos.com" created
INFO[0004]   Creating CustomResourceDefinition "installplans.operators.coreos.com"
INFO[0005]   CustomResourceDefinition "installplans.operators.coreos.com" created
INFO[0005]   Creating CustomResourceDefinition "olmconfigs.operators.coreos.com"
INFO[0006]   CustomResourceDefinition "olmconfigs.operators.coreos.com" created
INFO[0006]   Creating CustomResourceDefinition "operatorconditions.operators.coreos.com"
INFO[0007]   CustomResourceDefinition "operatorconditions.operators.coreos.com" created
INFO[0007]   Creating CustomResourceDefinition "operatorgroups.operators.coreos.com"
INFO[0008]   CustomResourceDefinition "operatorgroups.operators.coreos.com" created
INFO[0008]   Creating CustomResourceDefinition "operators.operators.coreos.com"
INFO[0009]   CustomResourceDefinition "operators.operators.coreos.com" created
INFO[0009]   Creating CustomResourceDefinition "subscriptions.operators.coreos.com"
INFO[0010]   CustomResourceDefinition "subscriptions.operators.coreos.com" created
INFO[0011] Creating OLM resources...
INFO[0011]   Creating Namespace "olm"
INFO[0012]   Namespace "olm" created
INFO[0012]   Creating Namespace "operators"
INFO[0013]   Namespace "operators" created
INFO[0013]   Creating ServiceAccount "olm/olm-operator-serviceaccount"
INFO[0014]   ServiceAccount "olm/olm-operator-serviceaccount" created
INFO[0014]   Creating ClusterRole "system:controller:operator-lifecycle-manager"
INFO[0015]   ClusterRole "system:controller:operator-lifecycle-manager" created
INFO[0015]   Creating ClusterRoleBinding "olm-operator-binding-olm"
INFO[0016]   ClusterRoleBinding "olm-operator-binding-olm" created
INFO[0016]   Creating OLMConfig "cluster"
INFO[0017]   OLMConfig "cluster" created
INFO[0017]   Creating Deployment "olm/olm-operator"
INFO[0018]   Deployment "olm/olm-operator" created
INFO[0018]   Creating Deployment "olm/catalog-operator"
INFO[0019]   Deployment "olm/catalog-operator" created
INFO[0019]   Creating ClusterRole "aggregate-olm-edit"
INFO[0020]   ClusterRole "aggregate-olm-edit" created
INFO[0020]   Creating ClusterRole "aggregate-olm-view"
INFO[0021]   ClusterRole "aggregate-olm-view" created
INFO[0021]   Creating OperatorGroup "operators/global-operators"
INFO[0022]   OperatorGroup "operators/global-operators" created
INFO[0022]   Creating OperatorGroup "olm/olm-operators"
 INFO[0023]   OperatorGroup "olm/olm-operators" created
INFO[0023]   Creating ClusterServiceVersion "olm/packageserver"
INFO[0024]   ClusterServiceVersion "olm/packageserver" created
INFO[0024]   Creating CatalogSource "olm/operatorhubio-catalog"
INFO[0025]   CatalogSource "olm/operatorhubio-catalog" created
INFO[0025] Waiting for deployment/olm-operator rollout to complete
INFO[0026]   Waiting for Deployment "olm/olm-operator" to rollout: 0 of 1 updated replicas are available
INFO[0052]   Deployment "olm/olm-operator" successfully rolled out
INFO[0052] Waiting for deployment/catalog-operator rollout to complete
INFO[0053]   Deployment "olm/catalog-operator" successfully rolled out
INFO[0053] Waiting for deployment/packageserver rollout to complete
INFO[0054]   Waiting for Deployment "olm/packageserver" to rollout: 0 of 2 updated replicas are available
INFO[0055]   Deployment "olm/packageserver" successfully rolled out
INFO[0055] Successfully installed OLM version "0.28.0"

NAME                                            NAMESPACE    KIND                        STATUS
catalogsources.operators.coreos.com                          CustomResourceDefinition    Installed
clusterserviceversions.operators.coreos.com                  CustomResourceDefinition    Installed
installplans.operators.coreos.com                            CustomResourceDefinition    Installed
olmconfigs.operators.coreos.com                              CustomResourceDefinition    Installed
operatorconditions.operators.coreos.com                      CustomResourceDefinition    Installed
operatorgroups.operators.coreos.com                          CustomResourceDefinition    Installed
operators.operators.coreos.com                               CustomResourceDefinition    Installed
subscriptions.operators.coreos.com                           CustomResourceDefinition    Installed
olm                                                          Namespace                   Installed
operators                                                    Namespace                   Installed
olm-operator-serviceaccount                     olm          ServiceAccount              Installed
system:controller:operator-lifecycle-manager                 ClusterRole                 Installed
olm-operator-binding-olm                                     ClusterRoleBinding          Installed
cluster                                                      OLMConfig                   Installed
olm-operator                                    olm          Deployment                  Installed
catalog-operator                                olm          Deployment                  Installed
aggregate-olm-edit                                           ClusterRole                 Installed
aggregate-olm-view                                           ClusterRole                 Installed
global-operators                                operators    OperatorGroup               Installed
olm-operators                                   olm          OperatorGroup               Installed
packageserver                                   olm          ClusterServiceVersion       Installed
operatorhubio-catalog                           olm          CatalogSource               Installed
```
