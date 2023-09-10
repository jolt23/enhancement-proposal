# enhancement-proposals

An Enhancement Proposal is a process to communicate and track new changes across an organization. The proposal process is currently in draft mode and could change in the future.

Please view the first EP as an example.

This proposal process is heavily influenced by the Kubernetes Enhancement Proposal (KEP) and is meant as a demonstration of how this process can be used to create a standardized way to communicate ideas and changes to an existing system.

## Getting Started with EPs

1. Discuss your EP within your team and department
2. Create a EP with the following template outlined [EP template](deps/template/README.md)

## FAQs

### Do I have to use the EP process?

Yes...

The EP process is meant to formalize the way changes are made to the system, platform or stack of technology and document why certain decisions were made. The power behind the EP is to make the process transparent and provide a mechanism for engineers to propose changes.

The git process allows EPs to be a living document that can receive feedback and go through rounds of reviews. This inturn documents why decisions were made and should help clarify requirements which are sometimes lost through time.

### Do EPs support multiple teams?

Yes, as this structure suggests you can have different teams or special interest groups separated to focus on specific portions of a system. This is great for systems which are complex and have different components that provide a unified experience. This is what makes the Kubernetes project so successful is the ability to have a singular vision but separated components to scale.

Not everyone outside of your group needs to be involved for a change, however if it is determined it will impact another team or group it is simple to tag them.

### How do I structure EPs

Typically you should think about the components that are separate across your system. Kubernetes refers to these as special interest groups which focus on specific parts of the system. However, within an organization this could be teams or a separation between api's and front end.

This means there is not one answer to how to structure your EPs however you should think about what constitutes a component as a whole. This process might require a broader conversation within an organization or project to come to an agreement on.
