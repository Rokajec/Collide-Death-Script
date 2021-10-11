using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEngine.SceneManagement;

public class TouchDeath : MonoBehaviour
{
    public GameObject Player;
    public int index;

    private void OnCollisionEnter2D(Collision2D other)
    {
        StartCoroutine(WaitBeforeShow());
    	//this is for it to wait few seconds before respawn
    }
    IEnumerator WaitBeforeShow()
    {
        Destroy(Player);
        yield return new WaitForSeconds(2);
        SceneManager.LoadScene(index);
    }

}
