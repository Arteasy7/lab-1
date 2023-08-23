public static Optional<UserGender> of(String gender) {
        for (UserGender userGender : values()) {
            if (userGender.gender.equals(gender)) {
                return Optional.of(userGender);
            }
        }
        return Optional.empty();
    }

    public static UserLevel of(int level) {
        for (UserLevel userLevel : values()) {
            if (userLevel.level == level) {
                return userLevel;
            }
        }
        return null;
    }
