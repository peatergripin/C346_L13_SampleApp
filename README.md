# 🌙 C346 Week07 Lesson13

[![Module](https://img.shields.io/badge/Module-C346%20Mobile%20App%20Development-6A5ACD?logo=android&logoColor=white)](#)
[![Platform](https://img.shields.io/badge/Platform-Android-2E8B57?logo=android&logoColor=white)](#)
[![Language](https://img.shields.io/badge/Language-JavaScript%20%7C%20React%20Native-61DAFB?logo=react&logoColor=white)](#)
[![Status](https://img.shields.io/badge/Status-Completed-success)](#)

---

## 📝 Overview

Lessons 13 & 14 taught us on the use of AsyncStorage.

> ✨ _Example:_ Implemented a persistent storage via the use AsyncStorage.

---

## 🎬 Demo / Media

<p align="center">
  <img src="./assets/img/screenshot1.png" width="180" alt="Screenshot1" />
</p>

---

## 🚀 Features

- ✅ AsyncStorage.getItem
- ✅ AsyncStorage.setItem

---

## 💡 Key Concepts

| Concept                  | Description                      |
| :----------------------- | :------------------------------- |
| **AsyncStorage.getItem** | Fetches data from Async Storage. |
| **AsyncStorage.setItem** | Stores item into Async Storage.  |

---

## 🧱 Code Snippet

```jsx
const getData = async () => {
  let datastr = await AsyncStorage.getItem("alphadata");
  if (datastr != null) {
    const jsondata = JSON.parse(datastr);
    setMydata(jsondata);
  } else {
    setMydata(datasource);
  }
};
getData();
```
