## Use Oculus ray interactor hover
```c#
using  Oculus.Interaction //from SDK declare header

private RayInteractor rayInteractor; //declare variables 

if (rayInteractor == null || !rayInteractor.HasCandidate)
{
    if (currentTargetObject != null)
    {
        Debug.Log("Unhovered: " + currentTargetObject.name);
        currentTargetObject = null;
    }
    return;
}

GameObject hovered = rayInteractor.Candidate.transform.gameObject;
if (hovered != currentTargetObject)
{
    currentTargetObject = hovered;
    OnRaycastHover(currentTargetObject);
}
```

## Use Oculus button
```c#
using OVR;
OVRInput.GetDown(OVRInput.Button.One); // A Button
```