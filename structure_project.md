# Food Hub Project Structure
food_hub/
├── assets/
│   ├── fonts/
│   ├── icons/
│   ├── images/
│   │   ├── auth/
│   │   ├── onboarding/
│   │   └── common/
│   └── translations/
│
├── lib/
│   ├── core/
│   │   ├── config/
│   │   │   ├── app_config.dart
│   │   │   ├── app_constants.dart
│   │   │   └── theme.dart
│   │   │
│   │   ├── errors/
│   │   │   ├── exceptions.dart
│   │   │   └── failures.dart
│   │   │
│   │   ├── local_storage/
│   │   │   ├── app_storage.dart
│   │   │   └── secure_storage.dart
│   │   │
│   │   ├── network/
│   │   │   ├── dio_provider.dart
│   │   │   └── interceptors.dart
│   │   │
│   │   ├── router/
│   │   │   └── app_router.dart
│   │   │
│   │   ├── services/
│   │   │   ├── camera_service.dart
│   │   │   ├── location_service.dart
│   │   │   └── permission_service.dart
│   │   │
│   │   ├── shared/
│   │   │   ├── buttons/
│   │   │   ├── dialogs/
│   │   │   ├── layout/
│   │   │   └── text_fields/
│   │   │
│   │   └── utils/
│   │       ├── currency_helper.dart
│   │       ├── date_formatter.dart
│   │       └── validators.dart
│   │
│   ├── features/
│   │   ├── auth/
│   │   │   ├── data/
│   │   │   │   ├── models/
│   │   │   │   │   ├── auth_response.dart
│   │   │   │   │   └── login_request.dart
│   │   │   │   ├── repositories/
│   │   │   │   │   └── auth_repository_impl.dart
│   │   │   │   └── sources/
│   │   │   │       ├── auth_api.dart
│   │   │   │       └── auth_local_source.dart
│   │   │   │
│   │   │   ├── domain/
│   │   │   │   ├── entities/
│   │   │   │   │   └── user_entity.dart
│   │   │   │   ├── repositories/
│   │   │   │   │   └── auth_repository.dart
│   │   │   │   └── usecases/
│   │   │   │       ├── login_usecase.dart
│   │   │   │       └── verify_otp_usecase.dart
│   │   │   │
│   │   │   └── presentation/
│   │   │       ├── providers/
│   │   │       │   └── auth_controller.dart
│   │   │       ├── screens/
│   │   │       │   ├── login_screen.dart
│   │   │       │   ├── reset_password_screen.dart
│   │   │       │   ├── sign_up_screen.dart
│   │   │       │   ├── verification_screen.dart
│   │   │       │   └── welcome_screen.dart
│   │   │       └── widgets/
│   │   │           └── otp_input_widget.dart
│   │   │
│   │   ├── cart/
│   │   │   ├── data/
│   │   │   │   ├── models/
│   │   │   │   ├── repositories/
│   │   │   │   └── sources/
│   │   │   ├── domain/
│   │   │   │   ├── entities/
│   │   │   │   ├── repositories/
│   │   │   │   └── usecases/
│   │   │   └── presentation/
│   │   │       ├── providers/
│   │   │       ├── screens/
│   │   │       │   └── cart_screen.dart
│   │   │       └── widgets/
│   │   │
│   │   ├── order/
│   │   │   ├── data/
│   │   │   │   ├── models/
│   │   │   │   ├── repositories/
│   │   │   │   └── sources/
│   │   │   ├── domain/
│   │   │   │   ├── entities/
│   │   │   │   ├── repositories/
│   │   │   │   └── usecases/
│   │   │   └── presentation/
│   │   │       ├── providers/
│   │   │       ├── screens/
│   │   │       │   ├── my_orders_screen.dart
│   │   │       │   └── review_restaurant_screen.dart
│   │   │       └── widgets/
│   │   │
│   │   ├── product/
│   │   │   ├── data/
│   │   │   │   ├── models/
│   │   │   │   │   ├── category_model.dart
│   │   │   │   │   └── food_model.dart
│   │   │   │   ├── repositories/
│   │   │   │   │   └── product_repository_impl.dart
│   │   │   │   └── sources/
│   │   │   │       └── product_api.dart
│   │   │   │
│   │   │   ├── domain/
│   │   │   │   ├── entities/
│   │   │   │   │   └── food_entity.dart
│   │   │   │   ├── repositories/
│   │   │   │   │   └── product_repository.dart
│   │   │   │   └── usecases/
│   │   │   │
│   │   │   └── presentation/
│   │   │       ├── providers/
│   │   │       │   ├── favorite_notifier.dart
│   │   │       │   └── home_notifier.dart
│   │   │       ├── screens/
│   │   │       │   ├── category_screen.dart
│   │   │       │   ├── favorites_screen.dart
│   │   │       │   ├── food_detail_screen.dart
│   │   │       │   └── home_screen.dart
│   │   │       └── widgets/
│   │   │           ├── banner_slider.dart
│   │   │           ├── category_item.dart
│   │   │           └── food_card.dart
│   │   │
│   │   └── profile/
│   │       ├── data/
│   │       │   ├── models/
│   │       │   ├── repositories/
│   │       │   └── sources/
│   │       ├── domain/
│   │       │   ├── entities/
│   │       │   ├── repositories/
│   │       │   └── usecases/
│   │       └── presentation/
│   │           ├── providers/
│   │           └── screens/
│   │               ├── address_screen.dart
│   │               ├── edit_profile_screen.dart
│   │               ├── profile_screen.dart
│   │               └── settings_screen.dart
│   │
│   ├── l10n/
│   │   ├── app_en.arb
│   │   ├── app_vi.arb
│   │   └── l10n.dart
│   │
│   ├── app.dart
│   ├── bootstrap.dart
│   └── main.dart
│
├── test/
│   ├── core/
│   └── features/
│
├── analysis_options.yaml
├── pubspec.yaml
└── README.md