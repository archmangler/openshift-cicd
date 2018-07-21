Notes gathered from readings across the openshift domain and ecosystem
======================================================================

1. "Source-to-Image
The true power of OpenShift comes in with the S2I (Source-to-Image) open source project that the OpenShift Team created as part of the OpenShift platform. The team knows that developers want to take advantage of all of the benefits that running appli‐ cations in containers provides, but don’t want to spend their day creating Dockerfiles or running Docker builds while also having to do all of the orchestration by hand.
In its simplest form, the S2I-based Docker images allow developers to interact with the platform from a pure source code perspective. What this means is that OpenShift only needs to know the URL of your git repository and then the platform takes care of the rest. Under the covers, when you create a new project and container, the plat‐ form matches a base image of the desired runtime up with your source, performs a build, and then creates a new Docker image on the fly."

(Openshift for Developers)

2. Kubernetes "Namespaces" vs openshift "Projects"

"The primary grouping concept in Kubernetes is the namespace. Namespaces, as the term suggests, provide a scope for names. More specifically, namespaces provide the scope named resources that describe your application and how it should be deployed. Namespaces are also a way to divide cluster resources between multiple uses. That being said, there is no security between namespaces in Kubernetes; if you are a “user” in a Kubernetes cluster, you can see all the different namespaces and the resources defined in them."

"The first new concept OpenShift adds is project, which effectively wraps a namespace, with access to the namespace being controlled via the project. Access is controlled through an authentication and authorization model based on users and groups. Projects in OpenShift therefore provide the walls between namespaces, ensuring that users, or applications, can only see and access what they are allowed to."


(Openshift for Developers)
