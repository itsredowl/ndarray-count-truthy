# 🌟 ndarray-count-truthy

![npm](https://img.shields.io/npm/v/ndarray-count-truthy) ![npm](https://img.shields.io/npm/dt/ndarray-count-truthy) ![GitHub](https://img.shields.io/github/license/itsredowl/ndarray-count-truthy)

Count the number of truthy elements along one or more ndarray dimensions.

---

## 📚 Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

---

## 📝 Introduction

The `ndarray-count-truthy` library provides a simple way to count truthy elements in ndarrays. Truthy values in JavaScript include any value that is not `false`, `0`, `""`, `null`, `undefined`, or `NaN`. This utility is particularly useful for data analysis, where you need to quickly assess the presence of valid data points.

---

## ⚙️ Installation

To install the package, use npm:

```bash
npm install ndarray-count-truthy
```

Alternatively, you can use yarn:

```bash
yarn add ndarray-count-truthy
```

---

## 📖 Usage

After installation, you can import the library into your JavaScript file:

```javascript
const countTruthy = require('ndarray-count-truthy');
```

You can then use the function to count truthy values in your ndarray.

---

## 🔍 API

### `countTruthy(arr, [axis])`

Counts the number of truthy elements in the provided ndarray.

#### Parameters

- **arr**: The input ndarray.
- **axis** (optional): The dimension along which to count truthy values. If not specified, it counts across all dimensions.

#### Returns

Returns an ndarray containing the counts of truthy elements.

---

## 📊 Examples

Here are some examples to illustrate how to use `ndarray-count-truthy`.

### Example 1: Basic Usage

```javascript
const ndarray = require('ndarray');
const countTruthy = require('ndarray-count-truthy');

const arr = ndarray([0, 1, 2, null, undefined, 'hello']);
const count = countTruthy(arr);

console.log(count); // Output: 3
```

### Example 2: Counting Along a Specific Axis

```javascript
const ndarray = require('ndarray');
const countTruthy = require('ndarray-count-truthy');

const arr = ndarray([[0, 1, 2], [null, 3, 4]]);
const count = countTruthy(arr, 0);

console.log(count); // Output: [1, 2, 2]
```

### Example 3: Handling Multi-dimensional Arrays

```javascript
const ndarray = require('ndarray');
const countTruthy = require('ndarray-count-truthy');

const arr = ndarray([
  [[0, 1], [2, null]],
  [[3, 4], [undefined, 5]]
]);
const count = countTruthy(arr, 1);

console.log(count); // Output: [[1, 2], [1, 2]]
```

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions or improvements, please create an issue or submit a pull request. Here are some guidelines:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Submit a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🚀 Releases

For the latest releases, visit [Releases](https://github.com/itsredowl/ndarray-count-truthy/releases). Make sure to download the latest version to get the most recent features and fixes.

---

## 📦 Additional Resources

- [ndarray Documentation](https://github.com/njsmith/ndarray)
- [JavaScript Array Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

---

## 🛠️ Support

If you encounter any issues or have questions, please check the [Issues](https://github.com/itsredowl/ndarray-count-truthy/issues) section. You can also visit the [Releases](https://github.com/itsredowl/ndarray-count-truthy/releases) page for updates.

---

## 📈 Analytics

Understanding the performance of your code is crucial. You can integrate this library into larger data analysis frameworks or use it in standalone scripts. The simplicity of counting truthy values can help streamline data cleaning and validation processes.

---

## 🎉 Acknowledgments

Thanks to the contributors of the `ndarray` library for providing a robust framework for handling multi-dimensional arrays. Your work makes projects like this possible.

---

## 🌐 Community

Join our community on GitHub Discussions or follow the project on social media for updates and tips. Share your experiences and use cases with `ndarray-count-truthy`!

---

Feel free to reach out if you have any questions or need assistance with the library. Your feedback helps improve the project.