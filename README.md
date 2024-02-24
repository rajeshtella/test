LocalDateTime localDateTime = LocalDateTime.now(); // Get current LocalDateTime

        // Specify the timezone (ZoneId)
        ZoneId zoneId = ZoneId.of("America/New_York"); // Example: New York timezone
        ZonedDateTime zonedDateTime = ZonedDateTime.of(localDateTime, ZoneId.systemDefault())
                .withZoneSameInstant(zoneId); // Convert LocalDateTime to ZonedDateTime and adjust to specified timezone

        System.out.println("ZonedDateTime: " + zonedDateTime);
