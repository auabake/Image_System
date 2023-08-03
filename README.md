# Image Sharing System

## Main System

![Pezesha](./Main.png)

The system will be running on AWS since its offers scalable and highly available infrastructure components, such as load balancers, auto-scaling, and managed databases.

System runs inside a Virtula Private Cloud. Request comming form users pass though API gateway this allows for load balancing and will be help full duirng auto scalling.

The API gateway handle authentication once authenticated the requests routed to the services.

## Application / User Service

This handles user data, accounts, profiles, friends lists, inbox and all related objects for the user.

## Image Service

Process the images before storage. The images are compressed and can be edited with filters, croped and image enhancements utilities.

## Image Storage

Making use of AWS object Storage with lifecycle to archive old images that havent been accesed for a number of days to save on storage costs.

## Data Storage

Usgin AWSRDS for postgress to hande user data. Maged service is earier to scale and maintinance.

## Security

![Pezesha](./Seurityp.png)


## Scalability

![Pezesha](./k8s.png)
