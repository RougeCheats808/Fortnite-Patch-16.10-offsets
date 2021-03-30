# Fortnite-Patch-16.10-offsets
Offsets pattern sigs

offsets



#pragma once

namespace addresses
{
	extern PVOID* uWorld;
	extern PVOID GetPlayerName;
	extern PVOID SetPawnVisibility;
	extern PVOID ClientSetRotation;
	extern PVOID ClientSetLocation;
	extern PVOID IsInVehicle;
	extern PVOID K2_TeleportTo;
	extern PVOID SetActorRelativeScale3D;
	extern PVOID AddYawInput;
	extern PVOID AddPitchInput;
	extern PVOID GetVehicleActor;
	extern PVOID GetVehicle;
	extern PVOID K2_AttachToActor;
	extern PVOID SetForcedLodModel;
	extern PVOID LaunchCharacter;
	extern PVOID SetActorLocation;
	extern PVOID GetActorEnableCollision;
	extern PVOID SetActorEnableCollision;
	extern PVOID ECollisionEnabled;
	extern PVOID SetCollisionEnabled;
	extern PVOID SetControlRotation;
	extern PVOID SetFirstPersonCamera;
	extern PVOID K2_SetActorRelativeLocation;
	extern PVOID K2_SetActorLocationAndRotation;
	extern PVOID K2_AddRelativeLocation;
	extern PVOID K2_SetRelativeLocation;
	extern PVOID CreativeToggleFly;
	extern PVOID ServerCreativeToggleFly;
	extern PVOID K2_AttachTo;
	extern PVOID K2_SetWorldLocation;
	extern PVOID LaunchPawn;
	extern PVOID OnLaunchPawn;
	extern PVOID TeleportVehicle;
	extern PVOID TeleportPlayerPawn;
	extern PVOID K2_SetActorRotation;
	extern PVOID K2_SetActorRelativeRotation;
	extern PVOID K2_SetWorldRotation;
	extern PVOID ReloadTime;
	extern PVOID ClientSetRotation;

}



namespace offsets
{
	enum Main : uint64_t
	{
		UWorld = 0x9412AA0,
	};

	enum World : uint64_t
	{
		OwningGameInstance = 0x180,
		Levels = 0x138,
	};

	enum Level : uint64_t
	{
		AActors = 0x98,
	};

	enum GameInstance : uint64_t
	{
		LocalPlayers = 0x38,
	};

	enum Player : uint64_t
	{
		PlayerController = 0x30,
	};

	enum Controller : uint64_t
	{
		ControlRotation = 0x288,

	};

	enum PlayerController : uint64_t
	{
		AcknowledgedPawn = 0x2A0,
	};

	enum Pawn : uint64_t
	{
		PlayerState = 0x240,
	};

	enum Actor : uint64_t
	{
		RootComponent = 0x130,
		CustomTimeDilation = 0x98,
	};

	enum Character : uint64_t
	{
		Mesh = 0x280,
	};

	enum SceneComponent : uint64_t
	{
		RelativeLocation = 0x11C,
		ComponentVelocity = 0x140,
	};

	enum StaticMeshComponent : uint64_t
	{
		ComponentToWorld = 0x1C0,
		StaticMesh = 0x480,
	};

	enum SkinnedMeshComponent : uint64_t
	{
		CachedWorldSpaceBounds = 0x600,
	};

	enum FortPawn : uint64_t
	{
		bIsDBNO = 0x552,
		bIsDying = 0x538,
		CurrentWeapon = 0x5D0,
		LastFireTimeVerified = 0x900,
		LastFireTime = 0x8FC,
	};

	enum FortPickup : uint64_t
	{
		PrimaryPickupItemEntry = 0x2A8,
	};

	enum FortItemEntry : uint64_t
	{
		ItemDefinition = 0x18,
	};

	enum FortItemDefinition : uint64_t
	{
		DisplayName = 0x80,
		Tier = 0x64,
	};

	enum FortPlayerStateAthena : uint64_t
	{
		TeamIndex = 0xEC0,
	};

	enum FortWeapon : uint64_t
	{
		WeaponData = 0x378,
		AmmoCount = 0x974,
	};

	enum FortWeaponItemDefinition : uint64_t
	{
		WeaponStatHandle = 0x820,
	};

	enum FortProjectileAthena : uint64_t
	{
		FireStartLoc = 0x878,
	};

	enum FortBaseWeaponStats : uint64_t
	{
		ReloadTime = 0xFC,
	};
	enum BuildingContainer : uint64_t
	{
		bAlreadySearched = 0xC61,
	};


	enum BuildingWeakSpot : uint64_t
	{
		bActive = 0x238,
	};


	enum MeatballVehicleConfigs : uint64_t
	{
		BoostMinPushForce = 0x678,
		BoostTopSpeedForceMultiplier = 0x67C,
		BoostTopSpeedMultiplier = 0x680,
		LandTopSpeedMultiplier = 0x688,
		LandPushForceMultiplier = 0x68C,
		BoostSteeringMultiplier = 0x6CC,
		LandSteeringMultiplier = 0x6D4,
		LandMinSpeedSteeringAngle = 0x6D8,
		LandMaxSpeedSteeringAngle = 0x6DC,
	};

	enum FortRangedWeaponStats : uint64_t
	{
		Spread = 0x15C,
		SpreadDownsights = 0x160,
		StandingStillSpreadMultiplier = 0x164,
		AthenaJumpingFallingSpreadMultiplier = 0x16C,
		AthenaCrouchingSpreadMultiplier = 0x168,
		AthenaSprintingSpreadMultiplier = 0x21C,
		MinSpeedForSpreadMultiplier = 0x174,
		MaxSpeedForSpreadMultiplier = 0x178,
		RecoilHoriz = 0x200,
		RecoilVert = 0x1F0,
		RecoilDownsightsMultiplier = 0x21C,
	};

	BOOLEAN Initialize();
}
----------------------------------------------------------------------------------------------------------------

sigs 
SIGS: CalculateSpreadCaller \x0F\x57\xD2\x48\x8D\x4C\x24\x?\x41\x0F\x28\xCD\xE8\x00\x00\x00\x00\x48\x8B\x4D\xB0\x0F\x28\xF0\x48\x85\xC9\x74\x05\xE8\x00\x00\x00\x00\x48\x8B\x4D\x98\x48\x8D\x05\x?\x?\x?\x?\x48\x89\x44\x24\x?\x48\x85\xC9\x74\x05\xE8\x00\x00\x00\x00\x48\x8B\x4D\x88

Process Event : \x40\x55\x56\x57\x41\x54\x41\x55\x41\x56\x41\x57\x48\x81\xEC\x00\x00\x00\x00\x48\x8D\x6C\x24\x00\x48\x89\x9D\x00\x00\x00\x00\x48\x8B\x05\x00\x00\x00\x00\x48\x33\xC5\x48\x89\x85\x00\x00\x00\x00\x8B\x41\x0C\x45\x33\xF6\x3B\x05\x00\x00\x00\x00\x4D\x8B\xF8\x48\x8B\xF2\x4C\x8B\xE1\x41\xB8\x00\x00\x00\x00\x7D\x2A


CalculateShot : \x48\x89\x5C\x24\x00\x4C\x89\x4C\x24\x00\x55\x56\x57\x41\x54\x41\x55\x41\x56\x41\x57\x48\x8D\x6C\x24\x00\x48\x81\xEC\x00\x00\x00\x00\x48\x8B\xF9\x4C\x8D\x6C\x24\x00


CalculateSpread : \x83\x79\x78\x00\x4C\x8B\xC9\x75\x0F\x0F\x57\xC0\xC7\x02\x00\x00\x00\x00\xF3\x41\x0F\x11\x00\xC3\x48\x8B\x41\x70\x8B\x48\x04\x89\x0A\x49\x63\x41\x78\x48\x6B\xC8\x1C\x49\x8B\x41\x70\xF3\x0F\x10\x44\x01\x00\xF3\x41\x0F\x11\x00\xC3
----------------------------------------------------------------------------------------------------------------
pattern 

// GObjects
		auto addr = FindPattern(xorstr("\x48\x89\x05\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x40\x84\xF6"), xorstr("xxx????x????xxx"));
		//auto addr = FindPattern(xorstr(""), xorstr(""));
		objects = reinterpret_cast<decltype(objects)>(RELATIVE_ADDR(addr, 7));
		if (!addr) {
			MessageBox(0, L"GObjects", L"Failure", MB_OK | MB_ICONERROR);
			return FALSE;
		}
		
		//          48 8B 05 7E 38 79 05 4C 8D 34 CD
		// GetObjectName
		addr = FindPattern(xorstr("\x40\x53\x48\x83\xEC\x20\x48\x8B\xD9\x48\x85\xD2\x75\x45\x33\xC0\x48\x89\x01\x48\x89\x41\x08\x8D\x50\x05\xE8\x00\x00\x00\x00\x8B\x53\x08\x8D\x42\x05\x89\x43\x08\x3B\x43\x0C\x7E\x08\x48\x8B\xCB\xE8\x00\x00\x00\x00\x48\x8B\x0B\x48\x8D\x15\x00\x00\x00\x00\x41\xB8\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x48\x8B\xC3\x48\x83\xC4\x20\x5B\xC3\x48\x8B\x42\x18"), xorstr("xxxxxxxxxxxxxxxxxxxxxxxxxxx????xxxxxxxxxxxxxxxxxx????xxxxxx????xx????x????xxxxxxxxxxxxx"));
		GetObjectNameInternal = reinterpret_cast<decltype(GetObjectNameInternal)>(addr);
		if (!addr) {
			MessageBox(0, L"GetObjectName", L"Failure", MB_OK | MB_ICONERROR);
			return FALSE;
		}
		// Free
		addr = FindPattern(xorstr("\x48\x85\xC9\x74\x2E\x53\x48\x83\xEC\x20\x48\x8B\xD9\x48\x8B\x0D\x00\x00\x00\x00\x48\x85\xC9\x75\x0C"), xorstr("xxxxxxxxxxxxxxxx????xxxxx"));
		FreeInternal = reinterpret_cast<decltype(FreeInternal)>(addr);

		// CalculateProjectionMatrixGivenView
		addr = FindPattern(xorstr("\x45\x0F\x57\xC0\x45\x8B\x81\x00\x00\x00\x00"), xorstr("xxxxxxx????"));
		addr -= 0x280;
		MH_CreateHook(addr, CalculateProjectionMatrixGivenViewHook, (PVOID*)&CalculateProjectionMatrixGivenView);
		MH_EnableHook(addr);
		//  45 0F 57 C0 45 8B 81 ? ? ? ? ? ? ? ? ? ? ? ?

		// LineOfSightTo
		addr = FindPattern(xorstr("\x40\x55\x53\x56\x57\x48\x8D\x6C\x24\x00\x48\x81\xEC\x00\x00\x00\x00\x48\x8B\x05\x00\x00\x00\x00\x48\x33\xC4\x48\x89\x45\xE0\x49"), xorstr("xxxxxxxxx?xxx????xxx????xxxxxxxx"));
		LineOfSightToInternal = reinterpret_cast<decltype(LineOfSightToInternal)>(addr);
---------------------------------------------------------------------------------------------------------------

