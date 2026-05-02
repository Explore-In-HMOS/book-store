# Book Store

This book-store-dev project is a wearable watch application built for **HarmonyOS NEXT** wearable devices, developed using **ArkTS**, designed to help users manage and explore their personal books collection.

# Preview

<div>
<img src="./screenshots/1.png" width="24%"/>
<img src="./screenshots/2.png" width="24%"/>
<img src="./screenshots/3.png" width="24%"/>
<img src="./screenshots/4.png" width="24%"/>
</div>

# Use Cases

The following are the application's featured use cases:

1. The user can see the splash page
2. The user can see a menu for Book of the day, Books, and Games
3. The user can see a list of Books(title, page count, description, category, image) that comes from Google Books API
4. The user can see details of books
5. The user can see a book of the day
6. The user can play with the Games button to catch the button

# Technology

## Stack
- **Languages**: ArkTS
- **Frameworks**: HarmonyOS SDK 5.1.0(18)
- **Tools**: DevEco Studio Vers 5.1.0.842
- **Libraries**: @kit.ArkUI, @kit.RemoteCommunicationKit

## Setup

### API Key
This project uses the [Google Books API](https://developers.google.com/books). The API key is not included in the repository.

Open `entry/src/main/resources/base/element/string.json` and set the `api_key` value:

```json
{
  "name": "api_key",
  "value": "YOUR_GOOGLE_BOOKS_API_KEY_HERE"
}
```

# Directory Structure

The project structure is as follows:

   ```
entry/src/main/ets/
|---component
|---|---BookCardComponent
|---|---BookDetailCard
|---model
|---|---BookModel
|---|---BookService
|---|---ImagesModel
|---|---RSPModel
|---|---volModel
|---|---VolumeInfoModel
|---pages
|---|---BookDetailPage
|---|---BookOfDayPage
|---|---BooksPage
|---|---HomePage
|---|---Index
|---utils
|---|---Constants
|---|---RCP
|---viewmodel
|---|---BookViewModel
|---|---HomeViewModel
|---entryability
|---|---EntryAbility
|---entrybackupability
|---|---EntryBackupAbility
   ```

# Constraints and Restrictions

## Supported Devices

- Huawei Watch 5

## Permissions

1. ohos.permission.INTERNET

# License

BookStore is distributed under the terms of the MIT License
See the [LICENSE](./LICENSE) for more information.
