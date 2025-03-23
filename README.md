# 🍽️ Restaurant Recommendation API using Redis

## 🚀 Why Redis?

This project leverages Redis as an in-memory data store to provide a high-performance and efficient caching mechanism for restaurant recommendations.

- **In-memory storage** → Fast access to data.
- **Great as a cache** → Reduces database load.
- **Highly performant** → Handles high traffic efficiently.

## 📌 Project Overview

This API provides restaurant and cuisine data with powerful Redis-based caching and search capabilities.

### **Cuisines**

- `GET /cuisines` → Retrieves all cuisines.
- `GET /restaurants?cuisine=<cuisine>` → Retrieves restaurants for a specific cuisine.

### **Restaurants**

- `GET /restaurants?name=<name>` → Search for restaurants by name.
- `POST /restaurants` → Creates a new restaurant.
- `GET /restaurants/top-rated` → Retrieves a ranked list of restaurants by rating.
- `POST /restaurants/:id/reviews` → Adds a review to a restaurant.
- `GET /restaurants/:id/reviews` → Retrieves all reviews for a restaurant.
- `DELETE /restaurants/:id` → Deletes a specific restaurant.
- `GET /restaurants/:id/location` → Retrieves restaurant location details.

## 🔥 Redis Features Used

This project utilizes several Redis features for optimal performance:

- **Hashes** → Store structured restaurant data.
- **Lists** → Manage restaurant reviews.
- **Sets** → Categorize cuisines and restaurants.
- **Sorted Sets** → Rank restaurants by ratings.
- **Strings** → Cache frequently accessed data.
- **RediSearch** → Full-text search for restaurant names.
- **Bloom Filters** → Prevent duplicate restaurant entries.

## 🛠️ Tech Stack

- **Backend**: Node.js, Express
- **Database**: Redis
- **Programming Language**: TypeScript
- **ORM**: RedisJSON
- **Search Engine**: RedisSearch

## ⚡ Installation & Running the Project

Make sure you have **Node.js** and **Redis** installed on your machine.

### **1️⃣ Clone the repository**

```sh
git clone <your-repo-url>
cd <your-repo-folder>
```

### **2️⃣ Install dependencies**

```sh
npm install
```

### **3️⃣ Build the project**

```sh
npm run build
```

### **4️⃣ Start the server**

```sh
npm start
```

## 📌 API Endpoints

| Method | Endpoint                         | Description                           |
| ------ | -------------------------------- | ------------------------------------- |
| GET    | `/cuisines`                      | Get all available cuisines            |
| GET    | `/restaurants?cuisine=<cuisine>` | Get restaurants by cuisine            |
| GET    | `/restaurants?name=<name>`       | Search restaurants by name            |
| POST   | `/restaurants`                   | Create a new restaurant               |
| GET    | `/restaurants/top-rated`         | Get top-rated restaurants             |
| POST   | `/restaurants/:id/reviews`       | Add a review to a restaurant          |
| GET    | `/restaurants/:id/reviews`       | Retrieve all reviews for a restaurant |
| DELETE | `/restaurants/:id`               | Delete a restaurant                   |
| GET    | `/restaurants/:id/location`      | Get restaurant location               |


💡 **Contributions are welcome!** If you have suggestions, feel free to submit a pull request. Happy coding! 🎉

