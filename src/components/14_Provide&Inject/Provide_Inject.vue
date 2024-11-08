<script setup>
import { provide } from 'vue';
import ChildComponent from './ChildComponent.vue';
provide('name','alex')
provide('age',20)

// const grandChild = {
//   name:'Harry',
//   age:20,
//   gender:'male'
// }


provide('carsData',[
  {
    id: 1,
    make: "Toyota",
    model: "Camry",
    year: 2023,
    type: "Sedan",
    fuelType: "Gasoline",
    price: 30000,
    features: ["Bluetooth", "Rear Camera", "Blind Spot Monitoring"],
    rating: 4.7
  },
  {
    id: 2,
    make: "Tesla",
    model: "Model S",
    year: 2022,
    type: "Electric",
    fuelType: "Electric",
    price: 80000,
    features: ["Autopilot", "Full Self-Driving", "Long Range Battery"],
    rating: 4.9
  },
  {
    id: 3,
    make: "Ford",
    model: "Mustang",
    year: 2021,
    type: "Coupe",
    fuelType: "Gasoline",
    price: 55000,
    features: ["Leather Seats", "Remote Start", "Premium Audio"],
    rating: 4.6
  },
  {
    id: 4,
    make: "BMW",
    model: "X5",
    year: 2023,
    type: "SUV",
    fuelType: "Hybrid",
    price: 75000,
    features: ["All-Wheel Drive", "Panoramic Sunroof", "Navigation System"],
    rating: 4.8
  },
  {
    id: 5,
    make: "Honda",
    model: "Civic",
    year: 2020,
    type: "Sedan",
    fuelType: "Gasoline",
    price: 22000,
    features: ["Eco Mode", "Adaptive Cruise Control", "Lane Departure Warning"],
    rating: 4.5
  },
  {
    id: 6,
    make: "Audi",
    model: "Q7",
    year: 2022,
    type: "SUV",
    fuelType: "Diesel",
    price: 65000,
    features: ["Third-Row Seating", "All-Wheel Drive", "Touchscreen Display"],
    rating: 4.7
  },
  {
    id: 7,
    make: "Chevrolet",
    model: "Silverado",
    year: 2023,
    type: "Truck",
    fuelType: "Gasoline",
    price: 45000,
    features: ["Towing Package", "4-Wheel Drive", "Backup Camera"],
    rating: 4.4
  },
  {
    id: 8,
    make: "Mercedes-Benz",
    model: "E-Class",
    year: 2022,
    type: "Sedan",
    fuelType: "Gasoline",
    price: 70000,
    features: ["Ambient Lighting", "Heated Seats", "Premium Sound System"],
    rating: 4.8
  }
])

</script>

<template>
  <h1>Provide & Inject</h1>
  <ChildComponent/>
</template>



<style>

</style>
