mutation {
    accountUpdateMfaChallenge(
        challengeId: "<CHALLENGE_ID>",
        otp: "<OTP>"
    ) {
        _id
        _createdAt
        _updatedAt
        userId
        expire
        provider
        providerUid
        providerAccessToken
        providerAccessTokenExpiry
        providerRefreshToken
        ip
        osCode
        osName
        osVersion
        clientType
        clientCode
        clientName
        clientVersion
        clientEngine
        clientEngineVersion
        deviceName
        deviceBrand
        deviceModel
        countryCode
        countryName
        current
        factors
        secret
        mfaUpdatedAt
    }
}
