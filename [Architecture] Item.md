# Properties

    public class Item{
        private long id;
        private string name;
        private string description;
        private EnumItemType itemType;
        private int level;

        private List<ItemStats> itemStats;  
        private bool isBound;
        private bool isWearable;
    }

# Associated class
> Item Stats

    public class ItemStats{
        private EnumStats stateName;
        private int statsValue;
    }

> Enum Stats

    public enum EnumStats{
        STR = 1;
        // ... other to define
    }

> Enum Item Type

    public enum EnumItemType{
        //... other to define
        WEAPON_MELEE_SWORD = 10_000;
        WEAPON_RANGE_BOW = 11_000;
        ARMOR_LIGHT_HEADSET = 2_000;        
        ARMOR_MEDIUM_HEADSET = 3_000;        
        ARMOR_HEAVY_HEADSET = 4_000;
        ACCESSORY_RING
        ACCESSORY_EARING
        ACCESSORY_NECKLACE
        ACCESSORY_BELT
        GATHER_ORE
        GATHER_WOOD
        GATHER_PLANT
        GATHER_LEATHER
        GATHER_CLOTH

    }
