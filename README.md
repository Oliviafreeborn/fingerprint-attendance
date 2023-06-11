
# Web-based Attendance System with Authentication and Attendance Tracking - Olivia Freeborn

This project aims to develop a web-based attendance system that streamlines the authentication and attendance tracking process for educational institutions. The system will provide a user-friendly interface for both students and instructors, making attendance management more efficient and reliable.

The system will incorporate a web application that allows students to log in securely using their unique credentials, eliminating the need for manual roll call and paper-based attendance sheets. Upon logging in, students will have access to their personal dashboard where they can view their attendance records, receive notifications, and track their overall attendance progress.

Instructors, on the other hand, will have a separate login to access the system's administrative interface. From this interface, instructors can manage class details, create courses, add students to classes, and monitor attendance statistics in real-time. The system will generate comprehensive attendance reports that can be exported or printed for record-keeping purposes.

## Authors

- [@olivafreeborn](https://github.com/Oliviafreeborn)


## Tech Stack

**Client:** HTML, CSS, Javascript

**Server:** PHP

**Front-end framework:** Bootstrap (client-side)

**Database:** MySQL


## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### Biometric Authentication with Fingerprint

This API integrates the Biometric Web Authentication API, which allows websites to incorporate biometric authentication methods, including fingerprint scanning, into their web applications. It provides a standardized way to implement biometric authentication and enhances the security and user experience of web applications.

To utilize biometric authentication, follow these steps:


- Request biometric authentication:
`navigator.credentials.get({
  publicKey: {
    allowCredentials: [{
      type: 'public-key',
      id: new Uint8Array([/* Credential ID */]),
    }],
    userVerification: 'required',
    authenticatorSelection: {
      requireResidentKey: true,
      userVerification: 'required',
    },
  },
});`

- Capture and process the biometric data:
`const fingerprintData = /* Capture biometric data */;
// Process and verify the captured biometric data`

- Authenticate the user based on the biometric data:
`if (/* Biometric data is authenticated */) {
  // Allow access to the application
} else {
  // Display an error message or deny access
}`
## Screenshots

![App Screenshot 1](https://user-images.githubusercontent.com/36708000/173137057-5aad5420-7689-4d5e-aae0-df796154e993.png)


![App Screenshot 1](https://user-images.githubusercontent.com/36708000/173137075-81d7b66e-a5cc-4228-ab14-cecc465701d7.png)

