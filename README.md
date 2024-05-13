# 


public class Door : MonoBehaviour
{
    public enum DoorType { Up, Down, Right, Left, DoorMax };

    public Tilemap WallTilemap;
    public Tilemap BackTilemap;
    public Tilemap MoveableTilemap;

    public Tilemap MainWallTilemap;
    public Tilemap MainBackTilemap;
    public Tilemap MainMoveableTilemap;

    public Tile tile;

    public Transform StartPos;
    public Transform EndPos;

    public Vector3Int DoorStartIndex;
    public Vector3Int DoorEndIndex;

    public Vector3Int MainStartIndex;
    public Vector3Int MainEndIndex;

    public Vector2Int size;

    public GameObject NextRoom;

    public BoxCollider2D coll;
    public LayerMask PlayerMask;
    public DoorType type;

    public BoxCollider2D collision;
    public GameObject ParentSage;
    public Transform TeleportPos;

    public bool nowdoorlocked;
}
