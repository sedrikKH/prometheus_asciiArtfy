# Suggestion for AsciiArtify
# Kubernetes systems for local development

## Introduction
Kubernetes is a container management platform used to deploy, scale, and manage containerized applications. For on-premises Kubernetes development and testing, tools are used to create and manage Kubernetes clusters on a local computer.

In this document, we compare three tools for deploying Kubernetes clusters in a local environment: minikube, kind, and k3d. We will discuss their features, advantages, and disadvantages, and demonstrate the tool we recommend.

## Comparative table of pros and cons characteristics 

|                      | Minikube                                                                                                                                          | Kind                                                                                                          | K3d                                                                                                                                        |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Supported OCs        | Linux, macOS, Windows                                                                                                                             | Linux, macOS, Windows                                                                                         | Linux, macOS, Windows                                                                                                                      |
| Architecture         | x86-64, ARM                                                                                                                                       | x86-64, ARM                                                                                                   | x86-64, ARM                                                                                                                                |
| Automation           | Ability to automate with scripts and tools such as Helm.                                                                                          | Easy automation thanks to the built-in Docker API                                                             | Automation thanks to Docker API, quick creation and testing of clusters                                                                    |
| Additional functions | Built-in dashboard, the ability to use VM drivers (VirtualBox, KVM, etc.).                                                                        | Quick creation of clusters in Docker containers, ease of use                                                  | Using RKE, easy scaling and management                                                                                                     |
| Advantages           | Easy to use Quick to build Supports all core Kubernetes features                                                                                  | Quick to build Supports all core Kubernetes features Easy to automate                                         | Quick to build Supports all core Kubernetes features Easily automated Supports advanced features such as cluster monitoring and management |
| Disadvantages        | The chosen type of virtualization can affect performance Does not scale to large clusters Possible problems with resources on the local computer. | Can be complex to configure Does not support some advanced features such as cluster monitoring and management | Can be complex to set up Uses Docker, which can be risky from a licensing perspective                                                      |

## Demonstration
Using k3d

![using a color picker](/doc/img/623779.gif)

## Conclusions:

Minikube is a good option for local development and testing, but its capabilities are limited by scalability.

Kind is a good option for quickly setting up a local Kubernetes cluster, but it lacks additional features such as cluster monitoring and management.

For local Kubernetes development and testing, we recommend using k3d. It has the following advantages:
* Fast deployment.
* Supports all the basic features of Kubernetes
* Has additional features such as cluster monitoring and management
